# Naming Methods

Prefer the following formats:
  **[Verb], [Verb] + [Noun],[Verb] + [Adjective] + [Noun]**
Use PascalCase  

## Single Purpose of All Methods

### Methods should have a single purpose

 Otherwise they cannot be named well
 How to name a method that creates annual incomes report, downloads updates from internet and scans the system for viruses?
 **CreateAnnualIncomesReportDownloadUpdatesAndScanForViruses** is a nice name, right?

Methods that have multiple purposes (weak cohesion) are hard to be named
**Need to be refactored instead of named**

### Good

```C#
  LoadSettings,
  Show,
  LoadSettingsFile,
  FindNodeByPattern,
  ToString,
  PrintList
```

- Method names should answer the question:
- What does this method do?
- If you cannot find a good name for a method, think about whether it has a clear intent

### Bad

```C#
 Method1,
 DoSomething,
 HandleStuff,
 SampleMethod,
 DirtyHack,
 Student,
 Generator,
 Counter,
 White,
 Approximation,
 MathUtils
 ```

## Methods Returning a Value

Methods returning values should describe the returned value

### Good

 **ConvertMetersToInches**, not **MetersInches** or **Convert** or **ConvertUnit**. Meters2Inches is still acceptable

CalculateSinus is good but *Sinus* is still acceptable
Ensure that the unit of measure is obvious
Prefer **MeasureFontInPixels** to MeasureFont

## Consistency in Methods Naming

Use consistent naming in the entire project

```c#
LoadFile, LoadImageFromFile, LoadSettings, LoadFont, LoadLibrary, but not ReadTextFile
```

Use consistently the opposites at the same level of abstraction:
**LoadLibrary** vs. **UnloadLibrary**,but not  *FreeHandle*
**OpenFile** vs. **CloseFile**, but not  *DeallocateResource*
**GetName** vs. **SetName**, but not  *AssignName*

## The Length of Method Names

- How long could be the name of a method?
  - Public methods should have short well defined names.
  - Private methods should have longer descriptive names.
  - Don't abbreviate
  - Your IDE has autocomplete

### Good

```C#
LoadCustomerSupportNotificationService,
CreateMonthlyAndAnnualIncomesReport
```

### Bad

```C#
LoadCustSuppSrvc,
CreateMonthIncReport
```
