# Naming Boolean Variables

- Give to boolean variables names that imply **true** or **false** (Predicates)
- Use positive boolean variable names
- Incorrect example

``` C#
if(! NotFound){....}
```

## Good

```C#
HasPendingPayment,
CustomerFound,
ValidAddress,
PositiveBalance,
IsPrime
```

## Bad

```C#
NotFound,
FindCustomerById,
Player,
ProgramStop,
Run,
List,
IsUnsuccessfull
```
