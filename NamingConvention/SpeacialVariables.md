# Naming Special Variables

- Naming counters
  - Establish a convention, e.g. [Noun] + **'Count'**
  - Good: ticketsCount, customersCount
- State
  - Establish a convention, e.g. [Noun] + **'State'**
  - Good: **blogParseState**, **threadState**
- Variables with small scope and span
  - E.g. loop counters
  - Short names can be used, e.g. **index, i, u**

## Temporary Variables

- Do you really think **temporary** variables exist?
  - All variables in the program are temporary because are used temporary only during the program execution, right?
- Temporary variables should NOT always be named better than **temp** or **tmp**:

## Good

```C#
//Swap a[i] and a[j]
int oldValue = a[i];
a[i] = a[j];
a[j]= oldValue;

for (int i=0, len= user.Lenght; i < len; i++)
{
  if(i % 2 == 0)
  sum +=user[i].Weight;
}

class Student {
  public string firstName { get; set; }
}
```

## Incorect examples

```C#
//Swap a[i] and a[j]
int temp = a[i];
a[i] = a[j];
a[j]= temp;

class LingkedList {
  public int flag { get; set; }
}

class Student {
  public int i { get; set; }
}
```

### The Length of Variable Names

- How long could be the name of a variable?
  - Depends on the variable scope and live time
  - More "famous" variables should have longer and more descriptive name
