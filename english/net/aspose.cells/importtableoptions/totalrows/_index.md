---
title: ImportTableOptions.TotalRows
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets total row count to import from data source. 1 means all rows of given data source
type: docs
url: /net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Gets or sets total row count to import from data source. -1 means all rows of given data source.

```csharp
public int TotalRows { get; set; }
```

### Examples

```csharp
// Called: { IsFieldNameShown = false, InsertRows = true, TotalRows = 1, TotalColumns = 2 });
[Test]
        public void Property_TotalRows()
        {
            caseName = "testImportDataView_015";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells[0, 0].PutValue(10);
            cells.ImportData(dataview, 0, 0, new ImportTableOptions()
            { IsFieldNameShown = false, InsertRows = true, TotalRows = 1, TotalColumns = 2 });

            checkImportDataView_015(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + "testDataView.xls");            
            //workbook = new Workbook(Constants.destPath + "testDataView.xls");
            checkImportDataView_015(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "testDataView.xlsx");            
            //workbook = new Workbook(Constants.destPath + "testDataView.xlsx");
            checkImportDataView_015(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + "testDataView.xml", SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + "testDataView.xml");
            checkImportDataView_015(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + "testDataView.xls");
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


