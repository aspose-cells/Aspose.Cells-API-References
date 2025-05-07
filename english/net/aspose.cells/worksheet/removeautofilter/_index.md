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
[Test]
        public void Method_RemoveAutoFilter()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "AutoFilter/CellsJava42915.xls");
            Console.WriteLine(wb.Worksheets.Names[0].RefersTo);
            Assert.IsTrue(wb.Worksheets[0].HasAutofilter);
            //wb.Save(Constants.destPath + "CellsJava42915.xls");
            wb = Util.ReSave(wb, SaveFormat.Excel97To2003);// new Workbook(Constants.destPath + "CellsJava42915.xls");
            wb.Worksheets[0].RemoveAutoFilter();
            Assert.IsFalse(wb.Worksheets[0].HasAutofilter);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


