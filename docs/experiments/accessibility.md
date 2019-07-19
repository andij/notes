---
description: Detailing the difference between implementations to choose the most appropriate solution
---

# Accessibility

## Using VoiceOver on iPhone

```markup
<a href="#!" target="_blank" rel="noopener" title="opens in a new window">some external page</a>
```

> Some external page. Link. _pause_ Opens in new window.

```markup
<a href="#!">take me somewhere</a>
```

> Take me somewhere. Link.

In this example an additional SVG image asset is used.

```markup
<a href="#" target="_blank" rel="noopener">some external page <img src="new-window.svg" alt="(opens in a new window)"></a>
```

> Some external page, Link.

Focus on the next item in the reading list.

> Opens in new window.

In this example an additional PNG image asset is used.

```markup
<a href="#" target="_blank" rel="noopener">some external page <img src="new-window.png" alt="(opens in a new window)"></a>
```

> Some external page, opens in a new window. Link.

```markup
<a href="#!" target="_blank" rel="noopener" data-alt="(opens in a new window)">some external page</a>
```

> Some external page, opens in a new window. Link.

```markup
<a href="#caveat" data-alt="Read further information within caveat item number">1</a>
```

> Read further information within caveat item number one. Link.

```markup
<a href="#!" target="_blank" rel="noopener" aria-label="opens in a new window">some external page</a>
```

> Opens in a new window. Link.

```markup
<a href="#!" target="_blank" rel="noopener">some external page<span class="sr-only">(opens in a new window)</span></a>
```

> Some external page, opens in a new window. Link.

```markup
<div hidden>
  <span id="new-window">Opens in a new window</span>
</div>
<a href="#!" target="_blank" rel="noopener" aria-describedby="new-window">some external page</a>
```

> Some external page. Link. _pause_ Opens in new window.