#### Rehydration Tips
### &nbsp;

## Responsiveness

- #### ember-responsive
- #### Use CSS

```hbs
  <div class="fg-col-md-4 hidden-xs hidden-sm map-column">

    {{#if (or media.isTabletLandscape media.isDesktop)}}
      {{search.map}}
    {{/if}}
    
  </div>
```
