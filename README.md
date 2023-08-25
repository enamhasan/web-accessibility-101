# web-accessibility-101
Web Accessibility / ADA complaint Cheat Sheet

#  Tools to ensure web Accessibility

 * Wave 
* Google Lighthouse
* voice-over
* Power mapper

# How to make a button web accessible

```<button>``` VS ```<a>``` tag  in terms of web Accessibility

The <button> element should be used for any interaction that performs an action on the current page. 
The <a> element should be used for any interaction that navigates to another view.

To make a button web-accessible
* Use Semantic HTML ```<button>``` tag with type attribute
* Use the aria-label Attribute to provide a more explicit label for assistive technologies. 
* Ensure the button is fully keyboard accessible. Users should be able to navigate to the button using the "Tab" key and activate it using the "Enter" or "Space"

### Example

 ``` <button type="button" aria-label="Click to submit the contact form">Send</button> ```

When you can’t use semantic HTML

``` <div role="button" tabindex="0" aria-label="Buy now, iPhone 17">Buy now </div> ```

# Make a background image web Accessible with Alt text

Do this:
```html
<div>
<span class="background-image" role="img" aria-label="[place alt text here]> </span>
[all the rest of my content]
</div>
```
Don't do this:
```
<div class="background-image" role="img" aria-label="blah blah blah">
[all the rest of my content]
</div>
```
Try not to use CSS for important informational images
For ambient images that are CSS, it is a courtesy to provide alternate text. When doing so, place image in its own empty<span> with an aria-label and role="img.This is also true, in a situation where CSS must be used for information content.
If the <div> with the CSS image absolutely MUST contain other content, then provide an empty <span> with an aria-label and role="img" immediately following the <div> that has the image.

# Make HTML Tab Accessible
![Accessible Tabs](https://github.com/enamhasan/web-accessibility-101/assets/9293561/4d5cdf00-1785-4cb1-a720-28c07377122b)
