---
title: ImportTableOptions.ConvertNumericData
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets a value that indicates whether the string value should be converted to numeric or date value
type: docs
url: /net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

```csharp
public bool ConvertNumericData { get; set; }
```

### Examples

```csharp
// Called: { IsFieldNameShown = true, InsertRows = true, ConvertNumericData = true });
[Test]
        public void Property_ConvertNumericData()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = getDataTable_String();
            cells[1048572, 0].PutValue(10);
            cells.ImportData(datatable, 1048572, 0, new ImportTableOptions()
            { IsFieldNameShown = true, InsertRows = true, ConvertNumericData = true });

            checkImportDataTable_Excel2007_008(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + &quot;testImportDataTable.xlsx&quot;);
            //workbook = new Workbook(Constants.destPath + &quot;testImportDataTable.xlsx&quot;);
            checkImportDataTable_Excel2007_008(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            //workbook.Save(Constants.destPath + &quot;testImportDataTable.xml&quot;, SaveFormat.SpreadsheetML);
            //workbook = new Workbook(Constants.destPath + &quot;testImportDataTable.xml&quot;);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;testImportDataTable.xls&quot;);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


