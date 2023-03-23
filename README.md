# boostrap

A "navbar" is an area on a page that contains navigation components (links, buttons, etc) for getting to other pages of the website. 
A "nav" is an HTML element that is normally used to enclose other elements related to navigation

navbar - Navbars require a wrapping .navbar with .navbar-expand{-sm|-md|-lg|-xl|-xxl} for responsive collapsing 
.navbar-expand{-sm|-md|-lg|-xl|-xxl}- is used to make navbar elements horizontally aligned and responsive withthe length of screen.

The "navbar-nav" class is used to style the unordered list that contains the navigation items.
It sets the list items to display inline, and adds left and right margins to create spacing between the items.

<nav class="navbar navbar-expand-lg">
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

