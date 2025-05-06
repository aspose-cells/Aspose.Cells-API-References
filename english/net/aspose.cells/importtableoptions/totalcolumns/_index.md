---
title: ImportTableOptions.TotalColumns
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets total column count to import from data source. 1 means all rows of given data source
type: docs
url: /net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Gets or sets total column count to import from data source. -1 means all rows of given data source.

```csharp
public int TotalColumns { get; set; }
```

### Examples

```csharp
// Called: cells.ImportData(dataview, 65535, 255, new ImportTableOptions() { IsFieldNameShown = false, TotalRows = 1, TotalColumns = 1 });
[Test]
        public void Property_TotalColumns()
        {
            caseName = &quot;testImportDataView_008&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells.ImportData(dataview, 65535, 255, new ImportTableOptions() { IsFieldNameShown = false, TotalRows = 1, TotalColumns = 1 });

            checkImportDataView_008(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;testDataView.xls&quot;);            
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xls&quot;);
            checkImportDataView_008(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + &quot;testDataView.xlsx&quot;);            
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xlsx&quot;);
            checkImportDataView_008(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + &quot;testDataView.xml&quot;, SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xml&quot;);
            checkImportDataView_008(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;testDataView.xls&quot;);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


