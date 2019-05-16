# Naming Enumerations

Several formats are acceptable:
[Noun] or [Verb] or [Adjective]
**Use the same style for all members**

## Good

```C#
enum Day {Monday, Tuesday, Wednesday, …}
enum AppState {Running, Finished, …}
enum WindowState {Normal, Maximized, …}
```

## Bad

```C#
enum Color {red, green, blue, white}
enum PAGE_FORMAT {A4, A5, A3, LEGAL, …}
```
