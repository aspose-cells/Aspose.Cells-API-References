---
title: PivotTable.RefreshDataOnOpeningFile
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether Refresh Data when Opening File
type: docs
url: /net/aspose.cells.pivot/pivottable/refreshdataonopeningfile/
---
## PivotTable.RefreshDataOnOpeningFile property

Indicates whether Refresh Data when Opening File.

```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```

### Examples

```csharp
// Called: pt.RefreshDataOnOpeningFile = false;
public void PivotTable_Property_RefreshDataOnOpeningFile()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46857_";

    Workbook book = new Workbook(filePath + "a.xlsx");
    PivotTable pt = book.Worksheets[0].PivotTables[0];
    pt.RefreshData();
    pt.CalculateData();
    pt.RefreshDataOnOpeningFile = false;
    book.Save(CreateFolder(filePath) + "a_out.xlsx");

    Workbook wb = new Workbook(filePath + "Attachment 1.xlsm");
    foreach (Worksheet worksheet in wb.Worksheets)
    {
        //被切片隐藏的条目 没有去除掉，因为隐藏条目的PiovtField没有应用在透视表的区域里，所以刷新时没有起作用
        worksheet.RefreshPivotTables();
    }

    wb.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


