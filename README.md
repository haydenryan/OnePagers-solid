# OnePagers Solid Website Template

[![Donate Now](https://img.shields.io/badge/donate-now-brightgreen.svg)](https://donorbox.org/onepagers-themes) [![Beerpay](https://beerpay.io/haydenryan/OnePagers-gradient/badge.svg?style=plastic)](https://beerpay.io/haydenryan/OnePagers-gradient) [![license](https://img.shields.io/github/license/haydenryan/onepagers-solid.svg)](https://github.com/haydenryan/OnePagers-solid)
[![GitHub stars](https://img.shields.io/github/stars/haydenryan/onepagers-solid.svg?style=social&label=Star)](https://github.com/haydenryan/OnePagers-solid)[![GitHub forks](https://img.shields.io/github/forks/haydenryan/onepagers-solid.svg?style=social&label=Fork)](https://github.com/haydenryan/OnePagers-solid)[![GitHub watchers](https://img.shields.io/github/watchers/haydenryan/onepagers-solid.svg?style=social&label=Watch)](https://github.com/haydenryan/OnePagers-solid)[![GitHub followers](https://img.shields.io/github/followers/haydenryan.svg?style=social&label=Follow)](https://github.com/haydenryan)


#### View the demo (and project website): https://haydenryan.github.io/OnePagers-solid/

"Solid" is part of the [OnePagers](https://github.com/haydenryan/OnePagers) collection of sleek single-page website templates by [@HaydenRyan](https://github.com/haydenryan).

  - Fully responsive, based on Bootstrap
  - Valid HTML, clean coding, easy to customise
  - 148 colours included
  - FontAwesome 4.7.0 included

[![Screenshot 1](https://haydenryan.github.io/OnePagers-solid/screenshot.png)](https://donorbox.org/onepagers-themes)
[![Screenshot 2](https://haydenryan.github.io/OnePagers-solid/screenshot2.png)](https://donorbox.org/onepagers-themes)

# Table of contents
1. [What's Inside](#whats-inside)
2. [Installation](#installation)
3. [Changing Content](#changing-content)
    1. [Changing Section Names and Links](#changing-section-names-and-links)
4. [Changing the Colours](#changing-the-colours)
5. [Adding Extra Sections](#adding-extra-sections)
6. [Change navbar transparency](#change-navbar-transparency)

## Whats Inside
| Package | Website |
| ------ | ------ |
| Bootstrap | http://getbootstrap.com |
| Font Awesome | http://fontawesome.io |
| uiGradients | http://uigradients.com |
| Google Fonts | http://fonts.google.com

## Installation
[Download the latest release as a .zip archive](https://github.com/haydenryan/OnePagers-solid/archive/master.zip)
To install, simply upload the following files to your host:
- css/
  - colours.min.css
  - onepagers-solid.css
  - bootstrap-theme.min.css
  - bootstrap.min.css
- font-awesome/
  - upload this whole directory (if you're using Font Awesome icons)
- js/
  - bootstrap.min.js
- index.html

No other files are required for the template to work.

In index.html, you can **easily delete the demo content**. Start with deleting the Demo Colours - lines 97-915. Alternatively, search the code for the string DELETE THIS.
## Changing Content
The template is broken up into 4 sections, by default. To add more, read the documentation on [adding extra sections](#adding-extra-sections).

Each section's content is marked at the beginning with the tag ```<-- START SECTION x -->``` and at the end with ```<-- END SECTION x -->```.

For exmple, to replace the content in Section 2, change the content between ```<!-- START SECTION 2 -->``` and ```<-- END SECTION 2 -->``` in the main index.html file

### Changing Section Names and Links
By default, the sections are named ```section1```, ```section2``` etc. This results in the links for each section being labelled http://youraddresshere/#section1 This is pretty bland and you should change this.

To change the name of a section:
1. Change the bold section link in the navbar (~line 50)
```<li><a href="```**```#section2```**```">The Colours</a></li>```

2. Change the ID of the corresponding div, for example ```<div class="col-md-12 section deep-space1" id="```**```section2```**```">```


## Changing the Colours
To choose a colour, [visit the demo](https://haydenryan.github.io/OnePagers-solid/) and scroll to the "Colours" section. Each colour is listed with its class name. 

To change a section's colour, change its **last class** (this is where we place the colour class, by default). For example to change Section 2 from deep-space1 to aubergine2, change ```<div class="col-md-12 section ```**```deep-space1```**```" id="section2">
``` to ```<div class="col-md-12 section ```**```aubergine2```**```" id="section2">``` 


## Adding Extra Sections
To add an extra section, copy and paste the code below into **index.html AFTER** the tag ```<!-- END SECTION 4 -->```, making sure to change **INSERT_COLOUR_NAME** and **INSERT_SECTION_ID**:

```
<!-- START EXTRA SECTION -->
<div class="row">
<div class="col-md-12 section innershadow INSERT_COLOUR_NAME" id="INSERT_SECTION_ID">
<div class="col-md-1">
</div>
<div class="col-md-10">
<!-- START EXTRA SECTION CONTENT -->
<h1>Heading</h1><br>
<p class="lead">Lead Paragraph</p>
<p>Next Paragraph</p>
<!-- END EXTRA SECTION CONTENT -->
</div>
<div class="col-md-1">
</div></div></div>
<!-- END EXTRA SECTION -->
```

Don't forget to add the section to the navbar, for example:

```
<li><a href="#INSERT_SECTION_ID">Section Name</a></li>
```

## Change navbar transparency
Want to change the transparency of the navbar? It's easy! By default, it's set to 95% opaque.

Simply go to line 108 of ```css/onepagers-solid.css``` and edit the following code:
```  
background-color: rgba(34, 34, 34, 0.95) !important;
```
Changing **0.95** to a different value. If you want it to be completely opaque, change this to **1**. If you want to make it more transparent, change it to something like **0.5**. Have a play around!

License
----

GNU GPLv3 
