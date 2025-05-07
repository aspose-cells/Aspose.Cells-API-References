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
            //<Font Style="FONT-FAMILY: Arial;FONT-SIZE: 10pt;COLOR: #000000;">abc</Font>

            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("abc");
            cells["A2"].PutValue("aaa");
            Console.WriteLine(cells["A1"].HtmlString);
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsHtmlString = true;
            DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 2, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), cells["A1"].HtmlString);
        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


