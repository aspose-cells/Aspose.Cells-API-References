---
title: Worksheet.ActiveCell
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets the active cell in the worksheet
type: docs
url: /net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Gets or sets the active cell in the worksheet.

```csharp
public string ActiveCell { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("B2", workbook.Worksheets[0].ActiveCell);
public void Worksheet_Property_ActiveCell()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual("B2", workbook.Worksheets[0].ActiveCell);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual("B2", workbook.Worksheets[0].ActiveCell);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual("B2", workbook.Worksheets[0].ActiveCell);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


