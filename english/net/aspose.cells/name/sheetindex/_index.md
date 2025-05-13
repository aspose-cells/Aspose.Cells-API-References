---
title: Name.SheetIndex
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates this name belongs to Workbook or Worksheet. 0  Global name otherwise index to sheet onebased
type: docs
url: /net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

```csharp
public int SheetIndex { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(8,workbook.Worksheets.Names[0].SheetIndex);
public void Name_Property_SheetIndex()
{
    Workbook workbook = new Workbook(Constants.sourcePath + @"example.xls");
    Assert.AreEqual(8,workbook.Worksheets.Names[0].SheetIndex);
    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


