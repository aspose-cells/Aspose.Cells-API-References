---
title: ImportTableOptions.IsFieldNameShown
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether field name should be imported
type: docs
url: /net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Indicates whether field name should be imported.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Examples

```csharp
// Called: IsFieldNameShown = true,
[Test]
        public void Property_IsFieldNameShown()
        {
            caseName = "testImportDataView_Excel2007_015";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells[1048573, 0].PutValue(10);
            cells.ImportData(dataview, 1048573, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                InsertRows = true,
                TotalRows = 1,
                TotalColumns = 3,
                NumberFormats = BuildNumberFormats("0.00", 3)
            });

            checkImportDataView_Excel2007_015(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "testDataView.xlsx");            
            //workbook = new Workbook(Constants.destPath + "testDataView.xlsx");
            checkImportDataView_Excel2007_015(workbook);
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


