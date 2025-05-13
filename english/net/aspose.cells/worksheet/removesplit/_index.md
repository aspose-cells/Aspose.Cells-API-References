---
title: Worksheet.RemoveSplit
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Removes split window
type: docs
url: /net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Removes split window.

```csharp
public void RemoveSplit()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].RemoveSplit();
public void Worksheet_Method_RemoveSplit()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].Split();
    Assert.AreEqual(workbook.Worksheets[0].PaneState, PaneStateType.Split);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].PaneState, PaneStateType.Split);
    workbook.Worksheets[0].RemoveSplit();
    Assert.AreEqual(workbook.Worksheets[0].PaneState, PaneStateType.Normal);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


