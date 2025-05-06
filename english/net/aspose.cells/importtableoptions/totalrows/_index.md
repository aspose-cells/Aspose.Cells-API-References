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
// Called: { IsFieldNameShown = true, InsertRows = true, TotalRows = tbl.Rows.Count, TotalColumns = tbl.Columns.Count });
[Test]
        public void Property_TotalRows()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET43860.xlsx&quot;);
            Cells sourceCells = workbook.Worksheets[0].Cells;
            Color c0 = sourceCells[&quot;A1&quot;].GetStyle().ForegroundColor;
            DataTable tbl = CreateValidTable1();

            sourceCells.ImportData(tbl, 0, 0, new ImportTableOptions()
            { IsFieldNameShown = true, InsertRows = true, TotalRows = tbl.Rows.Count, TotalColumns = tbl.Columns.Count });
            Color c1 = sourceCells[&quot;A1&quot;].GetStyle().ForegroundColor;
            Assert.AreEqual(c0, c1);
            Util.ReSave(workbook, SaveFormat.Xlsx);
            //string output = Constants.destPath + &quot;CELLSNET43860.xlsx&quot;;
            //workbook.Save(output);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


