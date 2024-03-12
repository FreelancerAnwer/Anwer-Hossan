### Button CSS

<style>
:root{
/*HOVER GRAD COLOR*/
--theme-color1: #ae8fff;
--theme-color2: #7243f2;

```
/*HOVER SOLID COLOR*/
--theme-color3: #ffffff;

--theme-color4: #1d1729;
--bg-theme-color2: #7243f2;
--gradient-1: linear-gradient(to left, var(--theme-color1), var(--theme-color2));

```

}
/*Button Global style */
.btn-style-one.btn-style-skew .elementor-button{
-webkit-transform: skew(-12deg);
transform: skew(-12deg);
transform-origin: top right !important;
-webkit-transform-origin: top right !important;
margin-right: 8px;
}
.btn-style-one .elementor-button-text, .btn-style-one .elementor-button-icon{
z-index: 2;
}
.btn-style-one.btn-style-skew .elementor-button-text{
transform: skew(12deg) !important;
}
.btn-style-one .elementor-button:before,.btn-style-two .elementor-button:before{
position: absolute;
left: 0;
top: 0%;
height: 100%;
width: 100%;
content: "";
background-color: var(--theme-color3);
z-index: -1;
-webkit-transform: scale(0, 1);
transform: scale(0, 1);
-webkit-transform-origin: bottom left;
transform-origin: bottom left;
transition: -webkit-transform 500ms cubic-bezier(0.86, 0, 0.07, 1);
-webkit-transition: -webkit-transform 500ms cubic-bezier(0.86, 0, 0.07, 1);
transition: transform 500ms cubic-bezier(0.86, 0, 0.07, 1);
transition: transform 500ms cubic-bezier(0.86, 0, 0.07, 1), -webkit-transform 500ms cubic-bezier(0.86, 0, 0.07, 1);
-webkit-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);
transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);
}
.btn-style-one.hvr-dark .elementor-button:before{
background-color: var(--theme-color4)!important;
z-index: 0;
}
.btn-style-one .elementor-button:hover:before{
-webkit-transform-origin: top right;
transform-origin: top right;
-webkit-transform: scale(1, 1);
transform: scale(1, 1);
}
.btn-style-two .elementor-button{
-webkit-transform: skew(-12deg);
transform: skew(-12deg);
-webkit-transform-origin: bottom left;
transform-origin: bottom left;
}
.btn-style-two .elementor-button:before{
background: var(--gradient-1);
-webkit-transform-origin: top right;
transform-origin: top right;
}
.btn-style-two:hover .elementor-button:before {
-webkit-transform-origin: bottom left;
transform-origin: bottom left;
-webkit-transform: scale(1, 1);
transform: scale(1, 1);
}
</style>

### Button Classes

***Solid Button Hover Class***
btn-style-one btn-style-skew
***Gradient Button Hover Class***
btn-style-one btn-style-two btn-style-skew

### Sub-Title Class

sub-title

### Sub-Title Border

/* sub-title After Border */
.sub-title .elementor-heading-title:before {
position: absolute;
left: 100%;
top: 50%;
margin-top: -4px;
height: 2px;
width: 26px;
margin-left: 10px;
background: var(--gradient-1);
content: "";
}
.sub-title .elementor-heading-title:after {
position: absolute;
left: 100%;
top: 50%;
margin-top: -6px;
height: 6px;
width: 6px;
margin-left: 36px;
background: var(--gradient-1);
content: "";
border-radius: 50%;
}

### Service Animation CSS

/*Service Section */
.inner-box .icon, .inner-box .image img, .inner-box .text, .inner-box .title .elementor-heading-title {
-webkit-transition: all 300ms ease;
transition: all 300ms ease;
}
.inner-box:hover .icon{
-webkit-transform: rotate(180deg) scale(-1);
transform: rotate(180deg) scale(-1) !important;
}
.inner-box:after {
position: absolute;
left: 0;
top: 0;
height: 100%;
width: 100%;
background-color: var(--bg-theme-color2);
-webkit-transform: scale(0);
transform: scale(0);
-webkit-transform-origin: right bottom;
transform-origin: right bottom;
border-radius: 500px 0 0;
content: "";
-webkit-transition: all 300ms linear;
transition: all 300ms linear;
}
.inner-box:hover::after {
-webkit-transform: scale(1.5);
transform: scale(1.5);
}
.service-block-two.inner-box::after {
-webkit-transform-origin: left bottom!important;
transform-origin: left bottom!important;
border-radius: 0 500px 0 0!important;
}
.service-block-three.inner-box:after {
-webkit-transform-origin: right top;
transform-origin: right top;
border-radius: 0 0 0 500px;
}
.service-block-four.inner-box:after {
-webkit-transform-origin: left top;
transform-origin: left top;
border-radius: 0 0 500px 0;
}
.inner-box:hover .text, .inner-box:hover .title .elementor-heading-title{
color: #ffffff !important;
}
.inner-box:hover .image img {
-webkit-transform: scale(1.1);
transform: scale(1.1);
}
@media only screen and (max-width: 1024px){
.inner-box .service-block-image{
position: relative;
}
.elementor-absolute.icon{
position: relative !important;
}
}

### Service Classes

***Service 1 Inner 2 Class***
service-block-one inner-box
***Service 2 Inner 2 Class***
service-block-two inner-box
***Service 3 Inner 2 Class***
service-block-three inner-box
***Service 4 Inner 2 Class***
service-block-four inner-box
***Service Inner 3 Class***
service-block-image
***Service Inner 3 Image Class***
image
***Service Icon Class***
icon
***Service H3 Class***
title
***Service Text Class***
text

### Portfolio Animation CSS

/*Portfolio Section*/
.project-block .image-box .elementor-widget-container:after{
position: absolute;
left: 0;
bottom: 0;
height: 0;
width: 100%;
opacity: 0;
content: "";
background: -webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0)), to #7243f2);
background: linear-gradient(to bottom, rgba(255, 255, 255, 0) 0%, #7243f2 100%);
pointer-events: none;
z-index: 2;
-webkit-transition: all 500ms ease;
transition: all 500ms ease;
}
.project-block  .image-box:hover .elementor-widget-container:after {
height: 100%;
opacity: 1;
}
.project-block .image-box::after {
position: absolute;
left: 0;
bottom: 0;
height: 0%;
width: 100%;
content: "";
background-color: #ffffff;
pointer-events: none;
z-index: 2;
-webkit-transition: all 500ms ease;
transition: all 500ms ease;
}
.project-block:hover .image-box:after {
height: 20px;
opacity: 1;
}
.project-block .image-box img, .project-block .content-box{
transition: all 0.4s ease !important;
}
.project-block:hover .image-box img{
-webkit-transform: scale(1.1);
transform: scale(1.1) !important;
-webkit-filter: grayscale(1);
filter: grayscale(1) !important;
}
.project-block:hover .content-box{
bottom: 0;
}

### Portfolio Classes

***Single Block Class***
project-block
***Single Block > ImageBox Class***
image-box
***Single Block > Contentbox Class***
content-box

### FAQ CSS

/*FAQ Section*/
.upper-box::after {
position: absolute;
right: 0;
top: 100%;
margin-top: -280px;
height: 510px;
width: 510px;
background-color: #f5f5f9;
content: "";
z-index: -1;
border-radius: 0 0 0 500px;
}
.bg-inner-column:before {
position: absolute;
top: 0;
height: 100%;
left: -1000px;
right: 0;
width: auto!important;
background: linear-gradient(to left, #ae8fff, #7243f2);;
content: "";
}
.bg-inner-column .sub-title .elementor-heading-title:before {
background: #fff;
}
.bg-inner-column .sub-title .elementor-heading-title:after {
background: #fff;
}

### FAQ Class

upper-box

### About Section CSS

/*About Agency Section*/
.overlay-anim:after {
background: rgba(255, 255, 255, 0.3);
content: "";
position: absolute;
left: 0;
top: 0;
width: 100%;
height: 0;
opacity: 1;
z-index: 9;
pointer-events: none;
}
.overlay-anim:hover:after {
height: 100%;
opacity: 0;
-webkit-transition: all 400ms linear;
transition: all 400ms linear;
}
.founder-info img{
padding: 3px;
}

### Breadcrumb Link CSS

/*Breadcrumb Link CSS*/
.page-breadcrumb a .elementor-icon-list-text{
color: var(--theme-color2) !important;
}
.page-breadcrumb a:hover .elementor-icon-list-text{
color: var(--theme-color3) !important;
}

### Breadcrumb IconList CSS

/*Breadcrumb Link CSS*/
.page-breadcrumb a .elementor-icon-list-text{
color: var(--theme-color2) !important;
}
.page-breadcrumb a:hover .elementor-icon-list-text{
color: var(--theme-color3) !important;
}

# **Breadcrumb IconList Class**

 page-breadcrumb

### Additional Service CSS

/*Additional Service*/
.service-block .service-box:after {
position: absolute;
left: 0;
top: 0;
height: 100%;
width: 100%;
background-color: #ffffff;
content: "";
z-index: 0;
-webkit-transition: all 300ms linear;
transition: all 300ms linear;
}
.service-block .service-box .round, .service-block .service-box img, .service-block .service-box .elementor-heading-title{
transition: all 300ms linear;
}
.service-block .service-box:hover:after{
height: 0;
}
.service-block .service-box:hover .round{
opacity: 0.1!important;
}
.service-block .service-box:hover img{
filter: brightness(0) invert(1);;
}
.service-block .service-box:hover .elementor-heading-title{
color: #fff;
}

### Additional Service Classes

***Parent Container***
service-block
***Single Block***
service-box
***Spacer widget***
round

### Animation Classes

animationFramesOne
contactSwimmer
rotateme

### Animation Classes

animationFramesOne
contactSwimmer
rotateme

### Animation Classes

animationFramesOne
contactSwimmer
rotateme
