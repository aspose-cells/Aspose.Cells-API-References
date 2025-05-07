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
// Called: wb.Worksheets.ActiveSheetName = "Sheet1";
[Test]
        public void Property_ActiveSheetName()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSNET-49624.xlsx");
            wb.Worksheets.ActiveSheetName = "Sheet1";
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            wb.Save(_destFilesPath + "CELLSNET-49624.html", saveOptions);
            string text = File.ReadAllText(_destFilesPath + "CELLSNET-49624.html");
            Assert.IsTrue(text.IndexOf("overflow:hidden;'>西吉县党家岔湿地保护区管理处</td>") != -1);
            Assert.IsTrue(text.IndexOf("（一）加强<span style='display:none'") != -1);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


