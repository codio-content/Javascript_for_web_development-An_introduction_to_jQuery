In this challenge we will develop a news website, totally in JS.

{Check It!|assessment}(test-2450424510)

|||guidance

Solution :

```html
<!DOCTYPE html>
<html>
<head>
  <title>News site</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  
  <div id="header">
    Welcome on my news site, <span class="username"> </span>
  </div>
  <div id="container">
    Loading ...
  </div>
  <div id="footer">
    Copyright 2015, My news site.
  </div>
  
  
  <script src="jquery.js"></script>
  <script src="news.js"></script>
  <script>
    $(document).ready(function(){
      
      // your code here to set the .username
      $(".username").text("Your name here");
    
      getNews(function(news) {
        
        // your code here to empty the #container
        $("#container").empty();
        
        var news_count = news.length;
        for (var i=0;i<news_count;i++) {
          var news_item = news[i];
          
          //your code here to create entries in #container for each news item .
          var news_div ='<div class="news" id="'+news_item.id+'">'
          +'<div class="author"> '+news_item.author+' </div>'
          +'<div class="title"> '+news_item.title+' </div>'
          +'<a href="'+news_item.link+'"> '+news_item.link+' </a> </div>'
      
          //your code here to append the div to the #container
          $("#container").append(news_div);
          
        }
        
      })
    })
  
  </script>
  
</body>
</html>
```

|||
