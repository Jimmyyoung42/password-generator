# password-generator
Built with
Semantic HTML5 markup
CSS Flexbox
Mobile-first workflow
Vanilla JS (async/await)
What I learned
Initially, my passwords were using p tags. To achieve the second stretch goal, adding an event listener that runs the copy to clipboard function when passwords are clicked seems enough, but then keyboard users have no way of selecting the passwords (because p tags are not "tabbable"). So I decided to use button tags instead to make the passwords accessible to keyboard users.

I also refactored the "copy to clipboard" implementation in this project after finishing the Color Scheme Generator which uses the same components. Basically, I learned the importance of having fallbacks (in this case, having a fallback in case navigator.clipboard.writeText fails when the browser doesn't have access to the clipboard).

On a related note, we might not need a fallback if in the first place we used input tags for the passwords and used the document.execCommand("copy") approach for the copy to clipboard implementation. However, using input is not really semantic (since we're not asking users to type in passwords) and it would just be another workaround so we can use an already deprecated feature.
