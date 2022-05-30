# password-generator
Built with
 HTML5 markup
CSS Flexbox

Vanilla JS 


I also refactored the "copy to clipboard" implementation in this project after finishing the Color Scheme Generator which uses the same components.  I learned the importance of having fallbacks (in this case, having a fallback in case navigator.clipboard.writeText fails when the browser doesn't have access to the clipboard).
 We might not need a fallback if in the first place we used input tags for the passwords and used the document.execCommand("copy") approach for the copy to clipboard implementation. However, using input is not really semantic (since we're not asking users to type in passwords) and it would just be another workaround so we can use an already deprecated feature.
