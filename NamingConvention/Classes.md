# Naming Special Classes

## Attributes

- Add 'Attribute' as suffi
- Eample: WebServiceAttribute
- Incorrect eample: WebService

### Collection Classes

- Add 'Collection' as suffi
- Eample: StringsCollection
- Incorrect eample: ListOfStrings

## Eceptions

- Add 'Eception' as suffi
- Use informative name
- Eample: FileNotFoundEception
- Incorrect eample: FileNotFoundError

### Delegate Classes

- Add 'Delegate' or 'EventHandler' as suffi
- Eample: DownloadFinishedDelegate
- Incorrect eample: WakeUpNotification

## The Length of Class Names

- How long could be the name of a class / struct / interface / enum / delegate?
- The name should be as long as required
- Don't abbreviate the names if this could make them unclear
- Your IDE has autocomplete, right?

Class names shouldn't be too long especially if the are used in public api's

### Good

```C#
FileNotFoundEception, CustomerSupportNotificationService
```

### Bad

```C#
NFEception, CustSuppNotifSrvc
```
