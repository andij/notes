---
layout: base.njk
description:  Detailing the difference between implementations to choose the most appropriate solution.
---

# Accessibility

## `ns-selector`
I've been listening to `ns-selector` with the NVDA screenreader with Firefox on Windows 10 (apparently that's a popular combination) and I've got it to a place where I believe that it provides exactly what we are after.

I'll check it using IE11, Edge and Chrome to see if there's anything crazy happening.

The conclusion that I've come to is:

When visiting the page and not interacting with the mouse or keyboard, the screenreader will read out the page from start to finish exactly as we would.

When encountering the `ns-selector` it'll read this:

> This is the label
> This is the helper text
> Item one heading
> Item one subheading
> Item one paragraph
> `radio button not checked`
> `clickable` Item one label
>
> Item two heading
> Item two subheading
> Item two paragraph
> `radio button not checked`
> `clickable` Item two label


When I **initially** interact with the page using the `tab` key it'll read this:

> This is the label `grouping`
> This is the helper text
> Item one label `radio button not checked`
> Item one heading
> Item one subheading
> Item one paragraph
> `1 of 3`

Then I use the `tab` key to navigate to the next Item and it'll read this:

> Item two label `radio button not checked`
> Item two heading
> Item two subheading
> Item two paragraph
> `2 of 3`


### 1.

Morning mate.

I've been listening to our ns-selector with the NVDA screenreader with Firefox on Windows 10 (apparently that's a popular combination) and I've got it to a place where I believe that it provides exactly what we are after. :thumbsup: 
I'll check it using IE11, Edge and Chrome to see if there's anything crazy happening.

The conclusion that I've come to is:

When visiting the page and not interacting with the mouse or keyboard, the screenreader will read out the page from start to finish exactly as we would. When reading the `ns-selector` it'll read this:
------
This is the label
This is the helper text
Item one heading
Item one subheading
Item one paragraph
`radio button not checked`
`clickable` Item one label
------

When I initially interact with the page using the `tab` key it'll read this:
------
This is the label `grouping`
This is the helper text
Item one label `radio button not checked`
Item one heading
Item one subheading
Item one paragraph
`1 of 3`
------
Then I use the `tab` key to navigate to the next `ns-selector` and it'll read this:
------
Item two label `radio button not checked`
Item two heading
Item two subheading
Item two paragraph
`2 of 3`
------




## _blank`

### 1.

```html
<a href="#!" target="_blank" rel="noopener" title="opens in a new window">some external page</a>
```

_Using VoiceOver on iPhone_

> Some external page. Link. _pause_ Opens in new window.

### 2.

```html
<a href="#!">take me somewhere</a>
```

_Using VoiceOver on iPhone_

> Take me somewhere. Link.

### 3.

In this example an additional SVG image asset is used.

```html
<a href="#" target="_blank" rel="noopener">some external page <img src="new-window.svg" alt="(opens in a new window)"></a>
```

_Using VoiceOver on iPhone_

> Some external page, Link.

Manually focus on the next item in the reading list.

> Opens in new window.

### 4.

In this example an additional PNG image asset is used.

```html
<a href="#" target="_blank" rel="noopener">some external page <img src="new-window.png" alt="(opens in a new window)"></a>
```

_Using VoiceOver on iPhone_

> Some external page, opens in a new window. Link.

### 5.

```html
<a href="#!" target="_blank" rel="noopener" data-alt="(opens in a new window)">some external page</a>
```

_Using VoiceOver on iPhone_

> Some external page, opens in a new window. Link.

### 6.

```html
<a href="#caveat" data-alt="Read further information within caveat item number">1</a>
```

_Using VoiceOver on iPhone_

> Read further information within caveat item number one. Link.

### 7.

```html
<a href="#!" target="_blank" rel="noopener" aria-label="opens in a new window">some external page</a>
```

_Using VoiceOver on iPhone_

> Opens in a new window. Link.

### 8.

```html
<a href="#!" target="_blank" rel="noopener">some external page<span class="sr-only">(opens in a new window)</span></a>
```

_Using VoiceOver on iPhone_

> Some external page, opens in a new window. Link.

### 9.

Including `aria-describedby` to associate a separated piece of content

```html
<span hidden id="new-window">Opens in a new window</span>

<a href="#!" target="_blank" rel="noopener" aria-describedby="new-window">some external page</a>
```

_Using VoiceOver on iPhone_

> Some external page. Link. _pause_ Opens in new window.

### 10.

Here, I've tried to use our `<ns-icon>` component in the same way, but it doesn't render the content into the DOM, if we were to use this technique, we will need to include the functionality

```html
<a href="#!" target="_blank" rel="noopener" aria-describedby="ns-icon-new-window">some external page <ns-icon id="ns-icon-new-window">opens in a new window</ns-icon></a>
```

_Using VoiceOver on iPhone_

> Some external page. Link

