---
title: ExportTableOptions.ExportAsHtmlString
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Exports the html string value of the cells to the DataTable
type: docs
url: /net/aspose.cells/exporttableoptions/exportashtmlstring/
---
## ExportTableOptions.ExportAsHtmlString property

Exports the html string value of the cells to the DataTable.

```csharp
public bool ExportAsHtmlString { get; set; }
```

### Examples

```csharp
// Called: etOpt.ExportAsHtmlString = true;
[Test]
        public void Property_ExportAsHtmlString()
        {
            //&lt;Font Style=&quot;FONT-FAMILY: Arial;FONT-SIZE: 10pt;COLOR: #000000;&quot;&gt;abc&lt;/Font&gt;

            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;abc&quot;);
            cells[&quot;A2&quot;].PutValue(&quot;aaa&quot;);
            Console.WriteLine(cells[&quot;A1&quot;].HtmlString);
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsHtmlString = true;
            DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 2, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), cells[&quot;A1&quot;].HtmlString);
        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


