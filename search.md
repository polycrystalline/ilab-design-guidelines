---
layout: page
title: Search
permalink: /search/
---


Search inputs are special types of [inputs](http://semantic-ui.com/elements/input.html#action).
<div class="ui action input">
  <input type="text" placeholder="Search all products">
  <button class="ui blue icon button">
    <i class="search icon"></i>
  </button>
</div>
<br>

#### Code

<!-- Search with Category Filter -->
Notice the border radius on the search input and the right hand search button.

<form action="/" method="get">
  <div class="ui left action input">

    <div class="ui floating dropdown button initialized" tabindex="0">
      <div class="text">products</div>
      <i class="dropdown icon"></i>
      <div class="menu transition hidden">
        <div class="item active selected" value="p">products</div>
      </div>
    </div>
    <input id="q" name="q" placeholder="Search..." size="30" type="text" value="">
    <input id="" name="" type="hidden" value="p">
    <button class="ui icon button">
      <i class="search icon"></i>
    </button>
  </div>
</form>
<br>

To get the borders to look right on this search, add the following CSS:

```css
.ui.left.action.input input {
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
}
 
.ui.left.action.input input + button {
   border-top-right-radius: 0.285714rem;
   border-bottom-right-radius: 0.285714rem;
}
```

#### Guidelines
- If the primary means for interacting with the page is search, make sure it is prominent.
- Avoid using Semantic UI's fuzzy search. It's too loose on word distances and is not easily adjustable.
- Add placeholder text that provides context despite it being low contrast.

