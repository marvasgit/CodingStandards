# Naming Variables

## Variable names

- Should be in **camelCase**
  - Preferred form: **[Noun]**- or **[Adjective]** + **[Noun]**
  - Should explain the purpose of the variable
    - If you can't find good name for a variable check if it has a single purpose
    - Exception: variables with very small scope, e.g. the index variable in a 3-lines long for-loop
  - Names should be consistent in the project
  - Private Member variables should be prefixed with an underscore (_ferriePrice,_authCode,_name)
- The name should address the problem we solve, not to the means used to solve it
  - Prefer nouns from the business domain to computer science terms

## Good

```C#
firstName,
report,
config,
usersList ,
fontSize,
maxSpeed,
font,
startIndex,
endIndex,
charsCount,
configSettingsXml,
dbConnection,
createUserSqlCommand,
accounts,
customers,
customerAddress,
accountHolder,
paymentPlan,
vipPlayer
```

## Bad

```C#
foo,
bar,
p,
p1,
p2,
populate,
LastName,
last_name,
LAST_NAME,
convertImage,
moveMargin,
MAXSpeed,
__temp,
firstNameMiddleNameAndLastName
paymentsPriorityQueue,
playersArray,
accountsLinkedList,
customersHashtable
```
