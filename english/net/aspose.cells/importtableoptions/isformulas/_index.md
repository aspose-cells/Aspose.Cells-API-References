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
            workbook.Worksheets[0].Cells[&quot;A1&quot;].Formula = &quot;=B1&quot;;
            DataTable dt = new DataTable();
            dt.Columns.Add(&quot;abasdf&quot;);
            dt.Rows.Add(&quot;=HYPERLINK(\&quot;https:\\domain.com\&quot;)&quot;);
            ImportTableOptions options = new ImportTableOptions();
            //  options.InsertRows = true;
            options.IsFieldNameShown = true;
            options.IsFormulas = new bool[] { true };
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A2&quot;].Formula, &quot;=HYPERLINK(\&quot;https:\\domain.com\&quot;)&quot;);
            workbook.Save(Constants.destPath + &quot;Test170847.xlsx&quot;);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


