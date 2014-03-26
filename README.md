Skin-Generator
==============

Fetch the skin of any Minecraft player and convert it into a 2D image that's human-viewable (doesn't look like the skin file)

Usage
=====

To use this just upload it your web server and visit the page, example: `http://yourdomain.com/skin.php?player={name}`

You can easily use this in any page by just using an <img> tag, here is an example of how to use it in a page
```html
<div class="someclass">
    <p>charries96's Skin:</p><br />
    <img src="http://charries96.co.nf/skin.php?player=charries96">
</div>
```

Alternatively if you add this to your `.htaccess` document you can get a players skin by using `http://yourdomain.com/skin/{name}`

```
Options +FollowSymLinks
RewriteEngine On
RewriteRule ^skin/([^/]*)$ /skin.php?player=$1 [L]
```

Code example:
```html
<div class="someclass">
    <p>charries96's Skin:</p><br />
    <img src="http://charries96.co.nf/skin/charries96">
</div>
```
