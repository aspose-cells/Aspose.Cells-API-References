---
title: StyleFlag.StyleFlag
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag constructor. Constructs an object with all flags as false
type: docs
url: /net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Constructs an object with all flags as false.

```csharp
public StyleFlag()
```

### Examples

```csharp
// Called: worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });
public void StyleFlag_Constructor()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var worksheet = workbook.Worksheets["DataBase"];

    Style boldStyle = GetCellsBoldStyle(workbook);

    worksheet.Workbook.DefaultStyle = worksheet.Workbook.GetNamedStyle("CDMDefaultStyle");

    worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

    worksheet.Cells[9, 0].PutValue("Test");

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(worksheet.Cells[9, 0].GetStyle().Font.IsBold);
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


