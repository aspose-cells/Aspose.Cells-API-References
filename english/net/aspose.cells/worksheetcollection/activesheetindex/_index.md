---
title: WorksheetCollection.ActiveSheetIndex
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents the index of active worksheet when the spreadsheet is opened
type: docs
url: /net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Represents the index of active worksheet when the spreadsheet is opened.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Remarks

Sheet index is zero based.

### Examples

```csharp
// Called: worksheets.ActiveSheetIndex = worksheets[targetSheetName].Index;
[Test]
        public void Property_ActiveSheetIndex()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA43387/&quot;;
            string savePath = CreateFolder(filePath);

            String targetSheetName = &quot;S.19.01_W\u00E4hrungen&quot;;
            LoadOptions loadOptions = new LoadOptions();
            LoadFilter loadFilter = new CustomerLoadFilter();
            loadOptions.LoadFilter = loadFilter;

            Workbook workbook = new Workbook(filePath + &quot;input.xlsx&quot;, loadOptions);
            WorksheetCollection worksheets = workbook.Worksheets;
            worksheets.ActiveSheetIndex = worksheets[targetSheetName].Index;

            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            workbook.Save(savePath + &quot;out.html&quot;, saveOptions);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


