# [PWS Tabs jQuery Plugin](http://alexchizhov.com/pwstabs)<sup>[1.1.4](#version-114-19012015)</sup>

####PWS Tabs is a lightweight jQuery tabs plugin to create flat style tabbed content panels with some cool transition effects powered by CSS3 animations.

## Demo

Online demo: [http://alexchizhov.com/pwstabs](http://alexchizhov.com/pwstabs)

![Preview](http://alexchizhov.com/files/themes/ac/page-templates/pwstabs/pwstabs114.jpg)

## Documentation

### Getting Started

1) Include jQuery library and jQuery PWS Tabs plugin in the <strong>`<head>`</strong> section.
```html
<script src="//code.jquery.com/jquery-1.11.2.min.js"</script>

<link type="text/css" rel="stylesheet" href="jquery.pwstabs.css">
<script src="jquery.pwstabs-1.1.4.js"></script>
```

2) Create tabbed panels and use HTML5 `data-pws-*` attributes to specify the ID & Name for the tabs.

```html
<div class="hello_world">

   <div data-pws-tab="anynameyouwant1" data-pws-tab-name="Tab Title 1">Our first tab</div>
   <div data-pws-tab="anynameyouwant2" data-pws-tab-name="Tab Title 2">Our second tab</div>
   <div data-pws-tab="anynameyouwant3" data-pws-tab-name="Tab Title 3">Our third tab</div>

</div>
```

<strong>`data-pws-tab`</strong> is used to initiate the tab and as its ID.

<strong>`data-pws-tab-name`</strong> is used for a tab display name.


3) Call the plugin on the parent element to create a basic tabs interface with 100% width and 'scale' transition effect.
```js
jQuery(document).ready(function($){
   $('.hello_world').pwstabs();
});
```

4) Available parameters to customize the tabs plugin.
```js
jQuery(document).ready(function($){
   $('.hello_world').pwstabs({

      // scale / slideleft / slideright / slidetop / slidedown / none
      effect: 'scale', 
 
      // The tab to be opened by default
      defaultTab: 1,    
 
      // Set custom container width
      // Any size value (1,2,3.. / px,pt,em,%,cm..)
      containerWidth: '100%',

      // Tabs position: horizontal / vertical
      tabsPosition: 'horizontal',
 
      // Tabs horizontal position: top / bottom
      horizontalPosition: 'top',

      // Tabs vertical position: left / right
      verticalPosition: 'left',
 
      // Right to left support: true/ false
      rtl: false

   });        
});
```


<p>5) PWS Tabs Plugin supports <strong><a href="http://fortawesome.github.io/" title="Go to Font Awesome Website" target="_blank">Font Awesome 4.2.0</a></strong></p>

<p>5.1) Include Font Awesome stylesheet from assets directory:</p>

```html
<link type="text/css" rel="stylesheet" href="../assets/font-awesome-4.2.0/css/font-awesome.min.css">
```

<p>5.2) Use HTML5 <strong>`data-pws-tab-icon`</strong> attribute to set an icon. Icon names you can find here: <a href="http://fortawesome.github.io/Font-Awesome/icons/" target="_blank">Font Awesome Icons</a>.</p>

```html
<div class="hello_world">

<div data-pws-tab="anynameyouwant1" data-pws-tab-name="Tab Title 1" data-pws-tab-icon="fa-heart">Our first tab</div>;
<div data-pws-tab="anynameyouwant2" data-pws-tab-name="Tab Title 2" data-pws-tab-icon="fa-star">Our second tab</div>
<div data-pws-tab="anynameyouwant3" data-pws-tab-name="Tab Title 3" data-pws-tab-icon="fa-map-marker">Our third tab</div>

</div>
```


## Options

<table>
<thead>
<tr>
<th>Option</th>
<th>Default</th>
<th>Description</th>
<th>Available options</th>
<th>Type</th>
</tr>
</thead>
<tbody>
<tr>
<td>effect</td>
<td>scale</td>
<td>Transition effect</td>
<td>scale / slideleft / slideright / slidetop / slidedown / none</td>
<td>string</td>
</tr>
<tr>
<td>defaultTab</td>
<td>1</td>
<td>Which tab is chosen by default</td>
<td>Tab ID number starts with 1 (1,2,3..)</td>
<td>string</td>
</tr>
<tr>
<td>containerWidth</td>
<td>100%</td>
<td>Tabs container width</td>
<td>Any size value (1,2,3.. / px,pt,em,%,cm..)</td>
<td>number</td>
</tr>
<tr>
<td>tabsPosition</td>
<td>horizontal</td>
<td>Define tabs position</td>
<td>horizontal / vertical</td>
<td>string</td>
</tr>
<tr>
<td>horizontalPosition</td>
<td>top</td>
<td>Define Horizontal tabs position</td>
<td>top / bottom</td>
<td>string</td>
</tr>
<tr>
<td>verticalPosition</td>
<td>left</td>
<td>Define Vertical tabs position</td>
<td>left / right</td>
<td>string</td>
</tr>
<tr>
<td>rtl</td>
<td>false</td>
<td>Right to left support</td>
<td>true / false</td>
<td>boolean</td>
</tr>
</tbody>
</table>


## Changelog

### Version 1.1.4 (19.01.2015)
1) Added new effect: none. Good for eCommerce websites. Customers don't like to wait :)<br>
2) Font Awesome 4.2.0 Support => Tabs Icons


### Version 1.1.3 (18.01.2015)
1) Added tabsPosition settings: horizontal / vertical.<br>
2) Added verticalPosition settings: left / right.<br>
3) Updated stylesheets.<br>
4) Updated examples.

### Version 1.1.2 (17.01.2015)
1) Added RTL support.<br>
2) Added horizontalPosition settings: top / bottom.<br>
3) New examples with video, Google Maps and mixed content.

### Version 1.1.1 (16.01.2015)
1) Bug fix: added class selector to tabs controller ul element. Solved issue with ul elements in tabs content.
