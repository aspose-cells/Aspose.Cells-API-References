---
title: Range.IsBlank
second_title: Aspose.Cells for .NET API Reference
description: Range method. Indicates whether the range contains values
type: docs
url: /net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Indicates whether the range contains values.

```csharp
public bool IsBlank()
```

### Examples

```csharp
// Called: Assert.IsTrue(r.IsBlank());
public void Range_Method_IsBlank()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Aspose.Cells.Range r = cells.CreateRange("A1:C10");
    Assert.IsTrue(r.IsBlank());
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


