---
title: WorksheetCollection.ActiveSheetName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents the name of active worksheet when the spreadsheet is opened
type: docs
url: /net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Represents the name of active worksheet when the spreadsheet is opened.

```csharp
public string ActiveSheetName { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets.ActiveSheetName = "F-ER-07-02 Versie 0.09";
public void WorksheetCollection_Property_ActiveSheetName()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    wb.Worksheets.ActiveSheetName = "F-ER-07-02 Versie 0.09";
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.ExportActiveWorksheetOnly = true;
    wb.Save(_destFilesPath + "example.html", saveOptions);
    string text = File.ReadAllText(_destFilesPath + "example.html");
    Assert.IsTrue(text.IndexOf("&nbsp;*Fout in procesfase <br/>&nbsp;") != -1);
    //

}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


