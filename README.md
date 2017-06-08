[![License](https://img.shields.io/github/license/sharedlabs/sortable-list.svg?style=flat-square)](https://github.com/sharedlabs/sortable-list/blob/master/LICENSE.md)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg?style=flat-square)](https://beta.webcomponents.org/element/sharedlabs/sortable-list)

_[Demo and API docs](https://sharedlabs.github.io/sortable-list/components/sortable-list/index.html)_

# sortable-list

`sortable-list` is a custom element that allows you sort element from a list by drag.

```html
<sortable-list on-sort-finish="_onSortFinish" dragging="{{dragging}}">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</sortable-list>

...
onSortFinish(event) {
  const sortedItem = event.detail.target;
}
```

When using a dom-repeat you must specify which items are sortable.
```html
<sortable-list sortable=".item">
  <dom-repeat>
    <div class="item"></div>
  </dom-repeat>
</sortable-list>
```

