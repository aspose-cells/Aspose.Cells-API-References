---
title: ImportTableOptions.IsFormulas
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether the data are formulas
type: docs
url: /net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

Indicates whether the data are formulas.

```csharp
public bool[] IsFormulas { get; set; }
```

### Examples

```csharp
// Called: options.IsFormulas = new bool[] { true };
[Test]
        public void Property_IsFormulas()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Formula = "=B1";
            DataTable dt = new DataTable();
            dt.Columns.Add("abasdf");
            dt.Rows.Add("=HYPERLINK(\"https:\\domain.com\")");
            ImportTableOptions options = new ImportTableOptions();
            //  options.InsertRows = true;
            options.IsFieldNameShown = true;
            options.IsFormulas = new bool[] { true };
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);
            Assert.AreEqual(workbook.Worksheets[0].Cells["A2"].Formula, "=HYPERLINK(\"https:\\domain.com\")");
            workbook.Save(Constants.destPath + "Test170847.xlsx");
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


