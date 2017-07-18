SuperEmbed.js
================
Live demo now available [here](https://corbindavenport.github.io/superembed.js).
---
SuperEmbed.js detects embedded videos from YouTube, Vimeo, Vine, VideoPress, DailyMotion, and more on webpages and makes them responsive. Essentially, this means they stretch to fill their container while still maintaining the content's original aspect ratio.

I created SuperEmbed to fix all my issues with existing solutions, including (but not limited to) unnecessary reliance on other libraries, bloated code, and poor fallback support.

**Features**
* Works without external libraries like JQuery
* Responsive videos maintain their original aspect ratio
* Responsive layout can be forced or blocked with classes applied to the embed code
* Extremely tiny, the minified version is only 3 KB

**Supported Services**

SuperEmbed can automatically detect and resize embedded content from these sites: 
* YouTube
* Vimeo
* SoundCloud
* Kickstarter
* CollegeHumor
* Hulu
* Flickr
* Vine
* VideoPress
* DailyMotion
* Twitch.tv
* Vid.me
* Facebook
* Gfycat
* LiveLeak
* MSDN Channel 9
* MySpace
* Archive.org

**Browser support**

| Chrome | Internet Explorer | Firefox | Safari | Opera |
| :-----:| :-----:| :-----:| :-----:| :-----:|
| 4.0+ | 9.0+ (see note) | 3.5+ | 3.2+ | 10+ |

*IE9 compatibility requires [classList.js](https://github.com/eligrey/classList.js), included in the 'extras' folder, to be loaded before SuperEmbed.js. This is not needed for IE10 and up.*

**How to use**

You can put the SuperEmbed script wherever you want on the page:
```
<script src="superembed.min.js"></script>
```
Then it will automatically resize any supported embedded videos. That's it.

*Note: If you already use JQuery, and you load SuperEmbed sometime after it, SuperEmbed will use JQuery to detect when the page is loaded and the window is resized (instead of DOM JavaScript).*

**Advanced features**

If you want to make an embedded video (or really any element) responsive, but it's not automatically detected by SuperEmbed, you can add the `.superembed-force` class to it like this:
```
<iframe src="http://www.example.com/video" class="superembed-force"></iframe>
```
You can also tell SuperEmbed to not resize a specific embed by adding the `.superembed-ignore` class, like this:
```
<iframe src="http://www.example.com/video" class="superembed-ignore"></iframe>
```
And finally, you can force a 1:1 aspect ratio by adding the `.superembed-square` class, like this:
```
<iframe src="http://www.example.com/video" class="superembed-square"></iframe>
```

---------------------------------------------------------

__New in SuperEmbed.js 3.1:__
* Added support for SoundCloud and MSDN Channel 9 embeds

---------------------------------------------------------

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
