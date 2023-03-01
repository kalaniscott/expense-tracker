<<<<<<< HEAD
# expense-tracker
Record expenses and visualize through time

node version 19.7.0
=======
# Budget Manager
Webapp to manage your budget and share budgets with others. Keep track of your balance sheet and avoid food spoilage.

## to-do list
- [ ] Create a database
- [ ] Create a server that can communicate with the database and feed processed data to the frontend
- [ ] Make an API call to Gmail to gather XML receipts
- [ ] Make a form to manually add an expense record
- [ ] Create an UI to access and visualize data
- [ ] Make a balance sheet viz
- [ ] Make a dynamic meal prep calendar 

## Balance sheet
An user has a records of `income` and `expense` at a given time.
The balance is the sumation of records within a range of time. This operation is recorded in time and its either scheduled or requested by user. 
`User` has many `Record` & `Balance`
`Balance` has many `Record`

```
Record {
 name: string,
 qty: number,
 currency: str,
 date: string,
 origin: string,
}
```

Records are saved for each user

| RecordID | date     | name     | qty     | currency |
|----------|----------|----------|---------|----------|
| 1        | 02-24-23 | salary   | 764     | usd      |
| 2        | 02-28-23 | rent     | -200000 | crc      |
| 3        | 02-18-23 | food     | -95000  | crc      |
| 4        | 02-28-23 | internet | -33000  | crc      |

### Income (Salary)
### Current Expenses
 - Food
 - Utility bills (water, electric, internet)
 - Rent
 - Gas
### Non-current expenses
 - Debt (credit card, loan)
 - Leisure (go-outs, drinks, etc)
### Balance
 - Net income
 - Savings

## Shared budgets
Users can create `budgets` which are groups of records from the user's balance. These budgets can be shared with other users.
 
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
 
 
>>>>>>> a773b3b220ac1b13fc18e9edcbd6045a792a2bcf
