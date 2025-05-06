---
title: ImportTableOptions.ColumnIndexes
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets the columns0based to import from data source. null means all columns should be imported
type: docs
url: /net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Examples

```csharp
// Called: options.ColumnIndexes = new int[] { 2 };
[Test]
        public void Property_ColumnIndexes()
        {
            caseName = &quot;testImportDataColumn_Excel2007_001&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = getDataTable();

            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 2 };
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            cells.ImportData(datatable, 1048575, 16383, options);

            checkImportDataColumn_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + &quot;testImportDataColumn.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testImportDataColumn.xlsx&quot;);
            checkImportDataColumn_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + &quot;testImportDataColumn.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testImportDataColumn.xml&quot;);
            workbook.Save(Constants.destPath + &quot;testImportDataColumn.xls&quot;);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


