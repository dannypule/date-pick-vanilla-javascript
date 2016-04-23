# Vanilla Javascript Date Picker
An open source date picker based on Material Design using vanilla javascript. 
Project initiated by Danny Pule www.dannypule.com

## -- STILL IN DEVELOPMENT --

 It can be used in any javascript based project and only has only one dependency which is the Roboto Google Font which is loaded using Javascript. To remove this font and use your own, see the below instructions in the 'Removing Roboto Font' section. 
 
COMPATABILITY

This date-picker should be compatible with all modern browsers including IE8 and IE9 which has been made compatible using a .classList polyfill made by Eli Grey called ClassList.js.
 
HOW TO USE THIS DATE PICKER IN YOUR OWN PROJECT

To include this dateicker, just copy the below files into your project:

date-pick.css

date-pick.js

Next, include the below line of code in any HTML file you intend to use this date picker:

````
<input id="date-picker-input" class="date-input" type="text" placeholder="Input a date"/>
````

Finally, give the input element that will be displaying the output of the date picker the below ID:
````
id="date-picker-input" 
````
 
REMOVING ROBOTO FONT 

To use your own font in the project, change the font family in the "#date-pick-container .date-pick" rule. Finally, remove this code from the Javascript file:
 ````
   WebFontConfig = {
      google: { families: [ 'Roboto::latin' ] }
    };
    (function() {
      var wf = document.createElement('script');
      wf.src = ('https:' == document.location.protocol ? 'https' : 'http') +
        '://ajax.googleapis.com/ajax/libs/webfont/1/webfont.js';
      wf.type = 'text/javascript';
      wf.async = 'true';
      var s = document.getElementsByTagName('script')[0];
      s.parentNode.insertBefore(wf, s);
    })();
  ````

The MIT License

Copyright (c) 2015-2016 Danny Pule, Inc. http://www.dannypule.com

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
