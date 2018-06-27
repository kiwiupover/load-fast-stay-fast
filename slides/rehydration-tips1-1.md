#### Rehydration Tips
### &nbsp;
## Move Ember Script Tags

```html
<body>
  {{content-for "body"}}

  <script src="assets/marketplace-search-vendor.js" defer></script>
  <script src="assets/marketplace-search.js" defer></script>

  {{content-for "body-footer"}}
</body>
```
