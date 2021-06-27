# Payment Protection Patterns
## 1. Check Effects Interaction
- Check conditions, check validity of parameters
- Change state variables
- Only interact with the other contracts last


## 2. Require msg.data.length == 0 in fallback function.
- Nothing should be executed aside from receiving ether

## 3. Avoid State changes in modifier

## 4. External calls are untrusted. Prefix function calling external calls with untrusted to write more test cases

## 5. Debit before credit

## 6. Functions should be private for those that handle transactions, unless being called by external

## 7. Separating app logic and data if possible, so that when changing the logic and redeploying, data won't be lost
