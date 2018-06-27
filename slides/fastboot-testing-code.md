##  fastboot testing

```js
it('serves pro-show page', function() {
  return this.visit('/pro/peacevans')
    .then(function(res) {
      let $ = res.jQuery;
      let response = res.response;
      let shoebox = JSON.parse($('#shoebox-pro-show').text());
      let shoeboxDataStore = JSON.parse($('#shoebox-ember-data-store').text());

      expect(response.statusCode).to.equal(200);
      expect($('head title').text()).to.equal('Peace Vans ....');
      expect($('#shoebox-pro-show').length).to.equal(1);
      expect(shoebox).to.have.any.keys('reviewIds', 'rentalIds', 'rentalsMeta');
      expect(shoeboxDataStore.records).to.have.any.keys('rental', 'image', 'user', 'review');
    });
});
```
