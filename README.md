# Budget Manager
Webapp to manage your budget and share budgets with others. Keep track of your balance sheet and avoid food spoilage.

## to-do list
- [ ] Make an API call to Gmail to gather XML receipts
- [ ] Make a form to manually add an expense record
- [ ] Create an UI to access and visualize data
- [ ] Make a balance sheet viz
- [ ] Make a dynamic meal prep calendar 

## Balance sheet
### Income

- Current Expenses
 - Food
 - Utility bills (water, electric, internet)
 - Rent
 - Gas
- Non-current expenses
 - Debt (credit card, loan)
 - Leisure (go-outs, drinks, etc)
- Balance
 - Net income
 - Savings
 
## Meal prepping
 
### Food inventory
Each food object represents an consumable expense, each Food() contains Nutrients() specified by a provider or accredited institution
 
### Meal library
Each meal is made of food portions

```
Meal { 
  name: string,
  ingridients: [ { food: Food(), portion_qty: int } ...rest ],
}

Meal("Pinto n eggs", [ FoodPortion("egg", 3), FoodPortion()
```
 
 
