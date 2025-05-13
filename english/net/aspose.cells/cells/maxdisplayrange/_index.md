---
title: Cells.MaxDisplayRange
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the max range which includes data merged cells and shapes
type: docs
url: /net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Gets the max range which includes data, merged cells and shapes.

```csharp
public Range MaxDisplayRange { get; }
```

### Remarks

Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.

### Examples

```csharp
// Called: Aspose.Cells.Range maxDisplay = worksheet.Cells.MaxDisplayRange;
public void Cells_Property_MaxDisplayRange()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47427/";

    Workbook workbook = new Workbook(filePath + "sample.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];

    Aspose.Cells.Range maxDisplay = worksheet.Cells.MaxDisplayRange;

    Aspose.Cells.Range toExport = worksheet.Cells.CreateRange(0, 0, 40, maxDisplay.ColumnCount);

    worksheet.PageSetup.PrintArea = toExport.Address;

    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.ExportPrintAreaOnly = true;
    saveOptions.ExportActiveWorksheetOnly = true;
    saveOptions.ExportImagesAsBase64 = true;
    saveOptions.ExportDataOptions = HtmlExportDataOptions.All;

    workbook.Save(CreateFolder(filePath) + "out.html", saveOptions);
}
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


