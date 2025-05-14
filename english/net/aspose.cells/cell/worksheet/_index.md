---
title: Cell.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the parent worksheet
type: docs
url: /net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Gets the parent worksheet.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: Assert.Fail(infoHead + cell.Worksheet.Name + "!" + cell.Name + ".GetDependents(): " + res);
private static void Cell_Property_Worksheet(string infoHead, Cell cell, string[] expected)
        {
            Cell[] leafs = cell.GetDependents(true);
            string res = CompareCollection.Compare(leafs == null ? null : leafs.GetEnumerator(),
                expected, new DependentComparator());
            if (res != null)
            {
                Assert.Fail(infoHead + cell.Worksheet.Name + "!" + cell.Name + ".GetDependents(): " + res);
            }
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


