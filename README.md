# Cat Squirrel Lounge

## Description
```
Cat Squirrel Lounge website is for fanciers of the Cat Squirrel.  In addition to t he classic blues harmonic riff made famous in Deep Purple's "My Woman from Tokyo". I hope to use the "cat squirrel"  Sciurus vulgaris a red squirrel native to europe as the ambassador of the nite club. Doctor Ross recorded the original Cat Squirrel in 1961. A song of unrequited love.



## Custom CSS Classes
```
The class(es) I created are:

1. class name ex( .main-info-section )
.column:first-child {border-style: solid}
.column:nth-child(2n+3) {border-style: dashed}
/* Responsive layout - makes a two column-layout instead of three columns */
@media screen and (max-width: 1024px) {
  .column {
    flex: 50%;
    max-width: 50%;
  }
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 512px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
}

2.

```



## Custom JavaScript Functions
```
The javascript functions I created are:

1* intended to toggle between displaying the images and displaying the information in the XMP tags metadata. */
function loadImageFiles ()
{
    console.log("tbd");
}

/* this was supposed to use the EXIF library to show the XMP meta data stored in the file, 
But I had trouble getting it to work */
function showXMP ()
{
var ilist = document.images;

for(var i = 0; i < ilist.length; i++) {
    alert(ilist[i].srcset);	
       /* display the img srcset files */
}	
}



window.onload = function() {
    var btn = document.getElementById("showImages");
    if (btn != null)
    	btn.onclick = loadImageFiles;
    var btn1 = document.getElementById("showXMP");
    if (btn1 != null)
    btn1.onclick = showXMP;
    
}
