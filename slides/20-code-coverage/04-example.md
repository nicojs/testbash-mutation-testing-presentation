```typescript
function isAllowedToBuyDrink(customer, drink) {
    if(drink.isAlcoholic) {
        return customer.age >= 18;
    } else {
        return true;
    }
}
```

```typescript
// Test
var customer = { name: 'Mark', age: 24 };
var beer = { name: 'Robo Beer', isAlcoholic: true };
var cola = { name: 'Roba cola', isAlcoholic: false };

expect(isAllowedToBuyDrink(customer, drink)).to.equal(true);
expect(isAllowedToBuyDrink(customer, drink)).to.equal(false);
```