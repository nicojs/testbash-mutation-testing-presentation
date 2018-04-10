<!-- .element: class="fragments-no-display"-->
### Mutating code

<pre><code data-noescape data-trim class="lang-js hljs javascript">
// Production code
function isAllowedToBuyDrink(customer, drink) {
    if(drink.isAlcoholic) {
        return <span class="fragment fade-out" data-fragment-index="2">customer.age <span class="fragment fade-out" data-fragment-index="0">>=</span><span class="fragment current-visible" data-fragment-index="0"><</span><span class="fragment fade-in" data-fragment-index="1">></span> 18</span><span class="fragment fade-in" data-fragment-index="2">true</span>;
        <span class="fragment current-visible" data-fragment-index="0">// mutated code, test FAILS</span><span class="fragment current-visible" data-fragment-index="1">// mutated code, test SUCCEEDS</span><span class="fragment current-visible" data-fragment-index="2">// mutated code, test SUCCEEDS</span>
    } else {
        return true;
    }
}
</code></pre>

<pre><code class="lang-js hljs javascript">// Test
var customer = { name: 'Mark', age: 24 };
var drink = { name: 'Robo Beer', isAlcoholic: true };

assert.equal(isAllowedToBuyDrink(customer, drink), true);
</code></pre>
