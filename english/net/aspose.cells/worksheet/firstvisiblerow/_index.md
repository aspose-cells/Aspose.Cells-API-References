---
title: Worksheet.FirstVisibleRow
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents first visible row index
type: docs
url: /net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Represents first visible row index.

```csharp
public int FirstVisibleRow { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(wb.Worksheets[2].FirstVisibleRow);
public void Worksheet_Property_FirstVisibleRow()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47593/";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "AS-ISK_v2_1.xlsm");
    Console.WriteLine(wb.Worksheets[2].FirstVisibleColumn);
    Console.WriteLine(wb.Worksheets[2].FirstVisibleRow);

    //wb.Save(filePath + "out.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExcludeUnusedStyles = true;
    options.ExportActiveWorksheetOnly = true;
    //options.ExportWorkbookProperties = false;
    //options.ExportWorksheetProperties = false;
    wb.Worksheets.ActiveSheetIndex = 2;

    wb.Save(savePath + "out.html", options);

    Workbook workbook = new Workbook(filePath + "sample.htm", new Aspose.Cells.HtmlLoadOptions());
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


