Super Swipebox
================================

A touchable jQuery lightbox.

[View project page](https://swipebox.codes/)

## What is Swipebox ?

Swipebox is a jQuery "lightbox" plugin for desktop, mobile and tablet.

## What's the difference between Super-Swipebox and the Original Swipebox ?

- Minimalism 1: all unnecessary files removed
- Minimalism 2: jQuery is already within the JS file to reduce chain file requests
- Firing the plugin happens already inside the JS file
- no class attributes needed. Just link to the JPG, GIF or PNG file
- double sized icons

## Features

- Swipe gestures for mobile
- Keyboard Navigation for desktop
- CSS transitions with jQuery fallback
- Retina support for UI icons
- Easy CSS customization
- Video, Images and Inline content

### Compatibility

Chrome, Safari, Firefox, Opera, IE9+, IOS4+, Android, windows phone.

## Usage

### Javascript

Include jquery and the swipebox script in your head tags or right before your body closing tag.

```html
<script src="swipebox/swipebox.js"></script>
```

### CSS

Include the swipebox CSS style in your head tags.

```html
<link rel="stylesheet" href="swipebox/swipebox.css">
```

### HTML

Just link the image (JPG, GIF or PNG) and optionally use the title attribute as caption.

```html
<a href="big/image.jpg" title="My Caption">
```

### Options

```javascript
useCSS : true, // false will force the use of jQuery for animations
initialIndexOnArray: 0, // which image index to init when a array is passed
removeBarsOnMobile : true, // false will show top navigation bar on mobile devices
hideCloseButtonOnMobile : false, // true will hide the close button on mobile devices
removeBarsOnMobile : true, // false will show bottom bar on mobile devices
hideBarsDelay : 3000, // delay before hiding bars on desktop
videoMaxWidth : 1140, // videos max width
beforeOpen: function(){} , // called before opening
afterOpen: null, // called after opening
afterClose: function(){}, // called after closing
afterMedia: function(){}, // called after media is loaded
loopAtEnd: false, // true will return to the first image after the last image is reached
autoplayVideos: false // true will autoplay Youtube and Vimeo videos
queryStringData: {} // plain object with custom query string arguments to pass/override for video URLs,
toggleClassOnLoad: '' // CSS class that can be toggled when the slide will be loaded (like 'hidden' of Bootstrap)
useSVG: true
nextSlide: function(){} // called on next slide, works for next button, arrow keys and touch navigation
prevSlide: function(){} // called on previous slide, works for previous button, arrow keys and touch navigation
```
