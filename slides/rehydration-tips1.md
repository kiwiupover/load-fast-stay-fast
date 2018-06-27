#### Rehydration Tips
### &nbsp;
## Title Tag

```js
export default Service.extend({
  headData: service(),
  
  setHeadTags() {
    set(this, 'titleTag', htmlSafe(`<title>${data.title}</title>`));
  }
});
```
