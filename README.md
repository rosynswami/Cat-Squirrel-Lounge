# Cat Squirrel Lounge

## Description
```
Cat Squirrel Lounge website is for fanciers of the Cat Squirrel.  In addition to t he classic blues harmonic riff made famous in Deep Purple's "My Woman from Tokyo". I hope to use the "cat squirrel"  Sciurus vulgaris a red squirrel native to europe as the ambassador of the nite club. Doctor Ross recorded the original Cat Squirrel in 1961. A song of unrequited love.



## Custom CSS Classes
```
The class(es) I created are:

/* General styles */

body {background-color: tomato;}
/*.debug {
border: 1px solid darkgrey;
}*/

img {max-width:100%;
	display: block;
} 

.row {
  display: flex;
  flex-wrap: wrap;
  padding: 0 6px;
  border: 6px solid #000;
}

* {
    box-sizing: border-box;
}

/* Create three equal columns that sits next to each other */
.column {
  flex: 33%;
  max-width: 33%;
  padding: 0 6px;
	border: 6px solid #000;
}

.column img {
  margin-top: 8px;
  vertical-align: middle;
}

.column:first-child {border-style: solid}
.column:nth-child(2n+3) {border-style: dashed}



/* Responsive layout - makes a two column-layout instead of three columns */
@media screen and (max-width: 1200px) {
  .column {
    flex: 50%;
    max-width: 50%;
  }
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 800px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
}

```



## Custom JavaScript Functions
```
The javascript functions I created are:


/* this one is supposed to set the image files style to show */
function loadImageFiles ()
{
    console.log("tbd");
}

/* This is supposed to be a toggle between showing the images and showing the srcset file URLs */
function showXMP ()
{
var ilist = document.images;

for(var i = 0; i < ilist.length; i++) {
   ilist[i].style.visibility = "show";
        // found the banner
}	
}


/* window onload handler */
window.onload = function() {
    var btn = document.getElementById("showImages");
    if (btn != null)
    	btn.onclick = loadImageFiles;
    var btn1 = document.getElementById("showXMP");
    if (btn1 != null)
    btn1.onclick = showXMP;
    
}
