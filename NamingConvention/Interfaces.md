# Naming Interfaces and Enumerations

## Naming Interfaces

Following formats are acceptable:
'I' + [Verb] + 'able'
'I' + [Noun], 'I' + [Adjective] + [Noun]

### Naming Interfaces Good

IEnumerable, IFormattable, IDataReader, IList, IHttpModule, ICommandExecutor

### Naming Interfaces incorrect examples

List, iFindUsers, IFast, IMemoryOptimize, Optimizer, FastFindInDatabase, CheckBox

## Naming Enumerations

Several formats are acceptable:
[Noun] or [Verb] or [Adjective]
**Use the same style for all members**

### Naming Enumerations Good

```C#
enum Day {Monday, Tuesday, Wednesday, …}
enum AppState {Running, Finished, …}
enum WindowState {Normal, Maximized, …}
```

### Naming Enumerations Bad

```C#
enum Color {red, green, blue, white}
enum PAGE_FORMAT {A4, A5, A3, LEGAL, …}
```
