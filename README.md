# turrell_3
<html>
    <head>
      <title>James Turrell 2</title>
      <script type="text/javascript" src="js_folder_path/moozoom.js"></script>
     </head>
    <body>
      
<a href="http://tinypic.com?ref=9bc677" target="_blank"><img src="http://i57.tinypic.com/9bc677.png" border="0" alt="Image and video hosting by TinyPic"></a>

var $win = $(window),
    w = 0,h = 0,
    rgb = [],
    getWidth = function() {
        w = $win.width();
        h = $win.height();
    };

$win.resize(getWidth).mousemove(function(e) {
    
    rgb = [
        Math.round(e.pageX/w * 255),
        Math.round(e.pageY/h * 255),
        150
    ];
    
    $(document.body).css('background','rgb('+rgb.join(',')+')');
    
}).resize();


      </body>
  </html>
