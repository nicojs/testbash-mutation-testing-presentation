### Mutation testing process
1. Mutate source code
2. Run tests for each mutation
3. Determine result:
    * Tests failed (good): Mutation 'killed'
    * Tests passed (bad): Mutation 'survived'
4. Calculate mutation score