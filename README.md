Gradient
======

use in server:

```coffeescript
Gradient = require('./gradient.js').Gradient

colors = Gradient.get '#12f3f4', '#fafcfa', 10

#colors is Array ['#12f3f4', ..., '#fafcfa'].lenght === 10
```

use in browser:
```html
<!DOCTYPE html>
<html>
<head>
<meta charset=utf-8 />
<title>JS Bin</title>
  <script src="http://code.jquery.com/jquery-1.9.1.min.js"></script>
</head>
<body>
  <div id="res">Run</div>
  <div>
  <ul id="id"></ul>
  </div>
  <script>
      var c = Gradient.get('#0000ac', '#ff9a9a', 10),
          i;

      for(i = 0; i < 10; i++) {
          $('<li>' + i + ' is color' + c[i] + '</li>').css('color', c[i]).appendTo('#id');
      }
  </script>
</body>
</html>
```
