# Naming Constants

- Use **CAPITAL_LETTERS** for **const** fields  and **PascalCase** for **readonly** fields
- Use meaningful names that describe their value

## Good

```C#
private const int READ_BUFFER_SIZE = 8192;
public static readonly PageSize DefaultPageSize = PageSize.A4;
private const int FONT_SIZE_IN_POINTS = 16;
```

## Bad

```C#
public const int MAX = 512; // Max what? Apples or Oranges?
public const int BUF256 = 256; // What about BUF256 = 1024?
public const string GREATER = "&gt;"; // GREATER_HTML_ENTITY
public const int FONT_SIZE = 16; // 16pt or 16px?
public const PageSize PAGE = PageSize.A4; // Maybe PAGE_SIZE?
```
