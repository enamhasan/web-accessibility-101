# web-accessibility-101
Web Accessibility / ADA complaint Cheat Sheet


# Make a background image web Accessible with alt text

Do this:
<div>
<span class="background-image" role="img" aria-label="[place alt text here]> </span>
[all the rest of my content]
</div>
Don't do this:
<div class="background-image" role="img" aria-label="blah blah blah">
[all the rest of my content]
</div>

>>Try not to use CSS for important informational images
>>For ambient images that are CSS, it is a courtesy to provide alternate text. When doing so, place image in its own empty<span> with an aria-label and role="img.This is also true, in a situation where CSS must be used for information content.
>>If the <div> with the CSS image absolutely MUST contain other content, then provide an empty <span> with an aria-label and role="img" immediately following the <div> that has the image.

