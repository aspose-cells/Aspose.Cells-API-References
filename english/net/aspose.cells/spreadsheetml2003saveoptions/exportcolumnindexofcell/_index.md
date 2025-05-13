---
title: SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetML2003SaveOptions property. The default value is false it means that column index will be ignored if the cell is contiguous to the previous cell
type: docs
url: /net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportColumnIndexOfCell = true;
public void SpreadsheetML2003SaveOptions_Property_ExportColumnIndexOfCell()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "HKG.xml");
    SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
    saveOptions.ExportColumnIndexOfCell = true;
    workbook.Save(Constants.destPath + "TestColumnIndex.xml");
}
```

### See Also

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


