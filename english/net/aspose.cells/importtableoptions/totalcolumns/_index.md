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
// Called: cells.ImportData(dataview, 1048575, 0, new ImportTableOptions() { IsFieldNameShown = false, TotalRows = 1, TotalColumns = 2 });
[Test]
        public void Property_TotalColumns()
        {
            caseName = "testImportDataView_Excel2007_006";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells.ImportData(dataview, 1048575, 0, new ImportTableOptions() { IsFieldNameShown = false, TotalRows = 1, TotalColumns = 2 });

            checkImportDataView_Excel2007_006(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "testDataView.xlsx");            
            //workbook = new Workbook(Constants.destPath + "testDataView.xlsx");
            checkImportDataView_Excel2007_006(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + "testDataView.xml", SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + "testDataView.xml");
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + "testDataView.xls");
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


