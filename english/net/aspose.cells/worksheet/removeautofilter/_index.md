---
title: Worksheet.RemoveAutoFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Removes the auto filter of the worksheet
type: docs
url: /net/aspose.cells/worksheet/removeautofilter/
---
## Worksheet.RemoveAutoFilter method

Removes the auto filter of the worksheet.

```csharp
public void RemoveAutoFilter()
```

### Examples

```csharp
// Called: wb.Worksheets[0].RemoveAutoFilter();
public void Worksheet_Method_RemoveAutoFilter()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xls");
    Console.WriteLine(wb.Worksheets.Names[0].RefersTo);
    Assert.IsTrue(wb.Worksheets[0].HasAutofilter);
    //wb.Save(Constants.destPath + "example.xls");
    wb = Util.ReSave(wb, SaveFormat.Excel97To2003);// new Workbook(Constants.destPath + "example.xls");
    wb.Worksheets[0].RemoveAutoFilter();
    Assert.IsFalse(wb.Worksheets[0].HasAutofilter);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


