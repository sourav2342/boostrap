# bootstrap

A "navbar" is an area on a page that contains navigation components (links, buttons, etc) for getting to other pages of the website. 
A "nav" is an HTML element that is normally used to enclose other elements related to navigation

navbar - Navbars require a wrapping .navbar with .navbar-expand{-sm|-md|-lg|-xl|-xxl} for responsive collapsing 
.navbar-expand{-sm|-md|-lg|-xl|-xxl}- is used to make navbar elements horizontally aligned and responsive withthe length of screen.

bg-light{navbar-light}- used for appending light background for navbar.

bootstarp has different colours light,primary,secondary,danger etc;more details
https://getbootstrap.com/docs/5.3/components/buttons/

navbar-barnd : used for differentaiting name of org in nav bar.

The "navbar-nav" class is used to style the unordered list that contains the navigation items.
It sets the list items to display inline, and adds left and right margins to create spacing between the items.

The "nav-item" class is used to define each item in the navigation list. It sets the display property to "inline-block", which allows the item to be positioned horizontally on the same line as the other navigation items.

The "nav-link" class is used to define the link within each navigation item. It sets the style of the link, such as color and font, and adds some padding to the link to make it easier to click.


<nav class="navbar navbar-expand-lg bg-light">
    
    <a class="navbar-brand" href="">contact</a>
    
    <ul class="navbar-nav">
         <li class="nav-item">
            <a class="nav-link" href="">contact</a>
         </li>
         <li class="nav-item">
           <a class="nav-link" href="">forum</a>
         </li>
         <li class="nav-item">
            <a class="nav-link" href="">patreon</a>
         </li>
    </ul>
</nav>

for adding space at the start of navbar elements /between navbar-brand and navbar elements we use space utility

NOTATION of using space utilities:

The classes are named using the format {property}{sides}-{size} for xs and {property}{sides}-{breakpoint}-{size} for sm, md, lg, xl, and xxl.

Where property is one of:

m - for classes that set margin
p - for classes that set padding
Where sides is one of:

t - for classes that set margin-top or padding-top
b - for classes that set margin-bottom or padding-bottom
s - (start) for classes that set margin-left or padding-left in LTR, margin-right or padding-right in RTL
e - (end) for classes that set margin-right or padding-right in LTR, margin-left or padding-left in RTL
x - for classes that set both *-left and *-right
y - for classes that set both *-top and *-bottom
blank - for classes that set a margin or padding on all 4 sides of the element
Where size is one of:

0 - for classes that eliminate the margin or padding by setting it to 0
1 - (by default) for classes that set the margin or padding to $spacer * .25
2 - (by default) for classes that set the margin or padding to $spacer * .5
3 - (by default) for classes that set the margin or padding to $spacer
4 - (by default) for classes that set the margin or padding to $spacer * 1.5
5 - (by default) for classes that set the margin or padding to $spacer * 3
auto - for classes that set the margin to auto

{property}{sides}-{size}
ms-auto
<ul class="navbar-nav ms-auto">

using Toggler to make navbar responsive to screen and to collapse the menu.ref
https://getbootstrap.com/docs/5.3/components/navbar/#toggler

  note: "With no .navbar-brand shown at the smallest breakpoint: what does that mean"
    If the ".navbar-brand" class is not shown at the smallest breakpoint, it means that the   brand/logo will not be displayed in the navbar when viewed on devices with small screens such as mobile phones.
   
    what is a smallest breakpoint?
    
      A breakpoint in web development is a specific point at which the layout of a website or web application changes in response to the size of the viewport or screen of the device on which it is being viewed.
    
    In other words, it is a specific width value where a website or web application changes its design to optimize its layout for that specific screen size.
    
    These breakpoints are usually defined in CSS using media queries. Media queries allow developers to write CSS rules that apply only when certain conditions are met, such as the width of the viewport being a specific value.
    
    
    a responsive nav-bar:
    
    /*<nav class="navbar navbar-expand-lg navbar-light bg-light">
    
    <a class="navbar-brand" href="">trunks</a>
    
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    
   <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
    <ul class="navbar-nav ms-auto">
         <li class="nav-item">
            <a class="nav-link" href="">contact</a>
         </li>
         <li class="nav-item">
           <a class="nav-link" href="">forum</a>
         </li>
         <li class="nav-item">
            <a class="nav-link" href="">patreon</a>
         </li>
    </ul>
   </div>
</nav>*/
    
 Bootstrap Grid layout
    
 <div class="row">
    <div class="col" style="background-color:red; border:1px solid;"> col </div>
    <div class="col" style="background-color:red; border:1px solid;"> col </div>
</div>
<div class="row">
    <div class="col-sm-6" style="background-color:red; border:1px solid;"> col </div>
    <div class="col-sm-6" style="background-color:red; border:1px solid;"> col </div>
</div>
    
    
    
Default container 

    Our default .container class is a responsive, fixed-width container, meaning its max-width changes at each breakpoint.


<div class="container">
  <!-- Content here -->
</div>
Responsive containers 

    Responsive containers allow you to specify a class that is 100% wide until the specified breakpoint is reached, after which we apply max-widths for each of the higher breakpoints. For example, .container-sm is 100% wide to start until the sm breakpoint is reached, where it will scale up with md, lg, xl, and xxl.


<div class="container-sm">100% wide until small breakpoint</div>
<div class="container-md">100% wide until medium breakpoint</div>
<div class="container-lg">100% wide until large breakpoint</div>
<div class="container-xl">100% wide until extra large breakpoint</div>
<div class="container-xxl">100% wide until extra extra large breakpoint</div>

Fluid containers 

    Use .container-fluid for a full width container, spanning the entire width of the viewport.


<div class="container-fluid">
  ...
</div>
    
if u want to add custom rules to conatiner-fluid use right cascaded order while giving links in html
   
    Cascading order: Make sure that your CSS rules are being applied in the correct order. CSS rules are applied in a cascading order, with later rules taking precedence over earlier rules. If there are conflicting rules for the same element, the last one defined will be applied.
    

    
    
