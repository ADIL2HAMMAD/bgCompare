# bgCompare.js
Use bgCompare to compare 2 images for differences, to create a before/after effect. 
It is fully responsive and works on all devices. It can even be put into a lightbox, 
like http://cornel.bopp-art.com/lightcase/. It is easy to set up anywhere.

DEMO : http://theflupke.github.io/bgCompare/

## Instructions

1. Link the css into the head of your html file
2. Link bgCompare.js just before the closing </body> tag
3. Add div container to body and configure bgCompare function for each slider. 

```html
<html>
  <head>
    ...
    <link href="css/bgCompare.min.css" rel="stylesheet" type="text/css" />
    ...
  </head>
  <body>
      ...
        <div id="bgCompare"></div>
      ...
     <script src="js/bgCompare.min.js"></script>
     <script>
       bgCompare({
          targetId:     "bgCompare",                                  // Your element id
          beforeImage:  "img/before-image.jpg", // Your before image
          afterImage:   "img/after-image.jpg",  // Your after image
        });
      </script>
   </body>
 </html>
```

##Options
```javascript
 bgCompare({
          beforeImage: "img/before.jpg", // Your before image
          afterImage: "img/after.jpg", // Your after image
          bgSize: "contain", // the background-size ("cover", "contain" for responsive awesomeness) (default "contain")
          targetId: "bgCompare", // the id of the element you want the script to load into
          showTooltips: "yes", // show or hide the tooltips next to the handle (default "yes")
          txtBefore: "Before", // the text of the before tooltip (default "Before")
          txtAfter: "After", // the text of the after tooltip (default "After")
          handleTheme: "dark-theme", // the theme of the handle (default "dark-theme")
          sliderPos: "20%" // the position of the slider on load (default: "50%")
        });
```
