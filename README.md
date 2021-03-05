Please keep track of any website you use; be it for research, design ideas, tutorials, etc.






-------------------------------------------------
How all the code I added works

The navigation bar works because of the style settings in style.css
the settings for

-ul {

-li a {

-li a.active {

-li a.inactive {

-li a:hover:not(.active) {


make the navigation bar work properly

The buttons on hotels.html are base on the design on the google doc, where clicking the button for the hotel one's staying at shows infromation for that location. 
The buttons work because of the following settings in style.css:

-.button {

-.button:hover {

-#myDIV {

-#myDIV2 {

-p.div {

-h3.div {


the .button and .button:hover deal with button appearence
the rest is for the divs that appear/disapear with the button click. The class p.div and h3.div are so the text in the menus that pop up can have different setting in the style sheet than the normal settings. do {p class="div"} {/p} and {h3 class="div"} {/h3} when writing in the hotel divs.

to add another button, you need to do the following ('_' is the number of button):

-make a new #myDIV_ in the style sheet (copy and paste the same style settings from the other id's)

-create another button with (button class="button" onclick="myFunction_())

-create a new div with (div id="myDIV_)

-create a new function called "myFunction_()".var x is the myDIV_ and the rest of the variables are the rest of the myDIVs. The if statement should set x to "block" and all other variables to "none" if the x = "none". The else should set x to "none".

-add "myFunction_()" to the (body onload="myFunction();myFunction2();etc...)

It could look like this:

-------------------------------------------------------
function myFunction2() {

  var x = document.getElementById("myDIV2);
  
  var y = document.getElementById("myDIV");
  
  var z = document.getElementById("myDIV3");
  
  if (x.style.display === "none") {
  
    x.style.display = "block";
    
    y.style.display = "none";
    
    z.style.display = "none";
    
  } else {
  
    x.style.display = "none";
    
  }
  
}
----------------------------------------------
since x = "myDIV2", this function is named "myFunction2()" and is triggered by the second button. 








