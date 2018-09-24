# Fix forms #

```
1. Insert after line:
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>

lines:
<link rel="stylesheet" href="http://ajax.googleapis.com/ajax/libs/jqueryui/1.12.1/themes/smoothness/jquery-ui.css">
<script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
<script>
    $(function() {
        var el=$("#sdate");
        el.datepicker();
    });
</script>


2. Change line:
<input name="sdate" type="date" value="">

to line:
<input name="sdate" type="text" id="sdate">


3. Remove line:
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.2/jquery.min.js"></script>
```
