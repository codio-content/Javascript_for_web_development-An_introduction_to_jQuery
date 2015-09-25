{Check It!|assessment}(test-3648361926)

|||guidance

Solution :

```
<script>
  $(document).ready(function(){
    
    for (var i=1;i<=10;i++) {
      //your code here.
      $("#container").append("<p>"+i+"</p>")

    }

    for (var j=1;j<=3;j++) {

      //your code here
      $("p").first().detach()

    }
    
  })
</script>
```

|||
