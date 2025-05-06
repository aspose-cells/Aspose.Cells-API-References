---
title: ImportTableOptions.InsertRows
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether new rows should be added for importing data records
type: docs
url: /net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Indicates whether new rows should be added for importing data records.

```csharp
public bool InsertRows { get; set; }
```

### Examples

```csharp
// Called: { IsFieldNameShown = false, InsertRows = false, TotalRows = 1, TotalColumns = 2 });
[Test]
        public void Property_InsertRows()
        {
            caseName = &quot;testImportDataView_016&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells[0, 0].PutValue(10);
            cells.ImportData(dataview, 0, 0, new ImportTableOptions()
            { IsFieldNameShown = false, InsertRows = false, TotalRows = 1, TotalColumns = 2 });

            checkImportDataView_016(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;testDataView.xls&quot;);            
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xls&quot;);
            checkImportDataView_016(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + &quot;testDataView.xlsx&quot;);            
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xlsx&quot;);
            checkImportDataView_016(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + &quot;testDataView.xml&quot;, SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + &quot;testDataView.xml&quot;);
            checkImportDataView_016(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;testDataView.xls&quot;);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


