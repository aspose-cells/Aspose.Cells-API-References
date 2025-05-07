---
title: ImportTableOptions.ImportTableOptions
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions constructor. Creates the default importing options
type: docs
url: /net/aspose.cells/importtableoptions/importtableoptions/
---
## ImportTableOptions constructor

Creates the default importing options.

```csharp
public ImportTableOptions()
```

### Examples

```csharp
// Called: cells.ImportData(dataview, 0, 0, new ImportTableOptions()
[Test]
        public void ImportTableOptions_Constructor()
        {
            caseName = "testImportDataView_018";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells.ImportData(dataview, 0, 0, new ImportTableOptions()
            { IsFieldNameShown = false, InsertRows = false, TotalRows = 0, TotalColumns = 0 });

            checkImportDataView_018(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + "testDataView.xls");            
            //workbook = new Workbook(Constants.destPath + "testDataView.xls");
            checkImportDataView_018(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "testDataView.xlsx");            
            //workbook = new Workbook(Constants.destPath + "testDataView.xlsx");
            checkImportDataView_018(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + "testDataView.xml", SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + "testDataView.xml");
            checkImportDataView_018(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + "testDataView.xls");
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


