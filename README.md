# Fix number #

```
1. Use:

<input type="text"
       class="form-control"
       style="width:100px; margin:10px;"
       placeholder="number"
       onkeyup="verify_number(this)">

2. Add javascript:

<script type="text/javascript">
    function verify_number(t) {
        if (t.value.match(/^(\d){1,10}$/g)) {
            t.setCustomValidity('')
            t.style.borderColor = ''
            t.style.boxShadow = ''
        } else {
            t.setCustomValidity('Wrong number')
            t.style.borderColor = '#FF0000'
            t.style.boxShadow = 'inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 8px rgba(255, 0, 0, 0.6)'
        }
    }
</script>
```

# Fix date #

```
1. Insert after line:
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>

lines:
<link rel="stylesheet" href="http://ajax.googleapis.com/ajax/libs/jqueryui/1.12.1/themes/smoothness/jquery-ui.css">
<script src="http://ajax.googleapis.com/ajax/libs/jqueryui/1.12.1/jquery-ui.js"></script>
<script>
    $(function() {
        $("#sdate").datepicker();
    });
</script>


2. Change line:
<input name="sdate" type="date" value="">

to:
<input type="text"
   name="sdate"
   class="form-control"
   style="width:100px; margin:10px;"
   placeholder="date"
   id="sdate">


3. Remove line:
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.2/jquery.min.js"></script>
```
