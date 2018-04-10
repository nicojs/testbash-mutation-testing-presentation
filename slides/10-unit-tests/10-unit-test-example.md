## Unit text example

```javascript
describe('PlaceOrderComponent', () => {
  it('should have 3 drinks', inject(($componentController) => {
    var ctrl = $componentController('roboPlaceOrder');
    expect(ctrl.drinks.length).toBe(3);
  }));
}); 
```

A JavaScript example using jasmine