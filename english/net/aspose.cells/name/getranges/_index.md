---
title: Name.GetRanges
second_title: Aspose.Cells for .NET API Reference
description: Name method. Gets all ranges referred by this name
type: docs
url: /net/aspose.cells/name/getranges/
---
## GetRanges() {#getranges}

Gets all ranges referred by this name.

```csharp
public Range[] GetRanges()
```

### Return Value

All ranges.

### Examples

```csharp
// Called: Aspose.Cells.Range[] ranges = recalculate ? name.GetRanges() : name.GetRanges(false);
private static void Name_Method_GetRanges(string msg, NameCollection names, bool recalculate)
        {
            int rc = 0;
            int nc = 0;
            foreach (Name name in names)
            {
                Aspose.Cells.Range[] ranges = recalculate ? name.GetRanges() : name.GetRanges(false);
                if (ranges != null)
                {
                    rc++;
                }
                else
                {
                    nc++;
                }
            }
            if (msg != null)
            {
                Console.WriteLine(msg + rc + ", " + nc);
            }
        }
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRanges(bool) {#getranges_1}

Gets all ranges referred by this name.

```csharp
public Range[] GetRanges(bool recalculate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |

### Return Value

All ranges.

### Examples

```csharp
// Called: Aspose.Cells.Range[] ranges = recalculate ? name.GetRanges() : name.GetRanges(false);
private static void Name_Method_GetRanges(string msg, NameCollection names, bool recalculate)
        {
            int rc = 0;
            int nc = 0;
            foreach (Name name in names)
            {
                Aspose.Cells.Range[] ranges = recalculate ? name.GetRanges() : name.GetRanges(false);
                if (ranges != null)
                {
                    rc++;
                }
                else
                {
                    nc++;
                }
            }
            if (msg != null)
            {
                Console.WriteLine(msg + rc + ", " + nc);
            }
        }
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


