# facebook-recommend-right
Workaround for Facebook Recommend social plugin to prevent it from overflowing when it is positioned to the right.

# how it works
It uses MutationObserver to catch opening the recommend box, then sets the outer div's dimension accordingly. 


* MutationObserver's adoptation level: caniuse.com/#search=MutationObserver
* a nice polyfill: https://github.com/megawac/MutationObserver.js/tree/master


Outer div has to be overflow:hidden to hide the recommend button, which prevents it from jumping around in the screen.
