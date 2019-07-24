---
description: Detailing the difference between implementations to choose the most appropriate solution
---

# Accessibility

## Using VoiceOver on iPhone

### 1.

```markup
<a href="#!" target="_blank" rel="noopener" title="opens in a new window">some external page</a>
```
_Using VoiceOver on iPhone_
> Some external page. Link. _pause_ Opens in new window.

### 2.

```markup
<a href="#!">take me somewhere</a>
```
_Using VoiceOver on iPhone_
> Take me somewhere. Link.

### 3.

In this example an additional SVG image asset is used.

```markup
<a href="#" target="_blank" rel="noopener">some external page <img src="new-window.svg" alt="(opens in a new window)"></a>
```
_Using VoiceOver on iPhone_
> Some external page, Link.

Manually focus on the next item in the reading list.
> Opens in new window.

### 4.

In this example an additional PNG image asset is used.

```markup
<a href="#" target="_blank" rel="noopener">some external page <img src="new-window.png" alt="(opens in a new window)"></a>
```
_Using VoiceOver on iPhone_
> Some external page, opens in a new window. Link.

### 5.

```markup
<a href="#!" target="_blank" rel="noopener" data-alt="(opens in a new window)">some external page</a>
```
_Using VoiceOver on iPhone_
> Some external page, opens in a new window. Link.

### 6.

```markup
<a href="#caveat" data-alt="Read further information within caveat item number">1</a>
```
_Using VoiceOver on iPhone_
> Read further information within caveat item number one. Link.

### 7.

```markup
<a href="#!" target="_blank" rel="noopener" aria-label="opens in a new window">some external page</a>
```
_Using VoiceOver on iPhone_
> Opens in a new window. Link.

### 8.

```markup
<a href="#!" target="_blank" rel="noopener">some external page<span class="sr-only">(opens in a new window)</span></a>
```
_Using VoiceOver on iPhone_
> Some external page, opens in a new window. Link.

### 9.

Including `aria-describedby` to associate a separated piece of content

```markup
<span hidden id="new-window">Opens in a new window</span>

<a href="#!" target="_blank" rel="noopener" aria-describedby="new-window">some external page</a>
```
_Using VoiceOver on iPhone_
> Some external page. Link. _pause_ Opens in new window.

### 10.

Here, I've tried to use our `<ns-icon>` component in the same way, but it doesn't render the content into the DOM, if we were to use this technique, we will need to include the functionality

```markup
<a href="#!" target="_blank" rel="noopener" aria-describedby="ns-icon-new-window">some external page <ns-icon id="ns-icon-new-window">opens in a new window</ns-icon></a>
```
_Using VoiceOver on iPhone_
> Some external page. Link
