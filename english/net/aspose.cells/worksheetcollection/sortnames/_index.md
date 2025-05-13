---
title: WorksheetCollection.SortNames
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Sorts the defined names
type: docs
url: /net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Sorts the defined names.

```csharp
public void SortNames()
```

### Remarks

If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving

### Examples

```csharp
// Called: wb.Worksheets.SortNames(); /*after this call, the button action is changed from the macro into "' Samleliste'!_FilterDatabase"*/
public void WorksheetCollection_Method_SortNames()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsm");
    wb.FileFormat = (FileFormatType.Excel97To2003); /*after this call the macro is included in worksheets.getNames();*/
    wb.Worksheets.SortNames(); /*after this call, the button action is changed from the macro into "' Samleliste'!_FilterDatabase"*/
    wb.Save(Constants.destPath + "example.xls");
    wb = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(wb.Worksheets[0].Shapes[1].MacroName, "CELLSJAVA42234.xls!Makro8");
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


