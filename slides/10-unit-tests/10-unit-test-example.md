## Unit text example

```javascript
// Production code
function isAllowedToBuyDrink(customer, drink) {
    if(drink.isAlcoholic) {
        return customer.age >= 18;
        
    } else {
        return true;
    }
}
```

```javascript
// Test
var customer = { name: 'Mark', age: 24 };
var drink = { name: 'Robo Beer', isAlcoholic: true };

expect(isAllowedToBuyDrink(customer, drink)).to.equal(true);
```

A JavaScript example using jasmine