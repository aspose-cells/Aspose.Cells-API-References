---
title: ImportTableOptions.ExportCaptionAsFieldName
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether exporting caption as field name
type: docs
url: /net/aspose.cells/importtableoptions/exportcaptionasfieldname/
---
## ImportTableOptions.ExportCaptionAsFieldName property

Indicates whether exporting caption as field name

```csharp
public bool ExportCaptionAsFieldName { get; set; }
```

### Remarks

Only works for DataTable.

### Examples

```csharp
// Called: options.ExportCaptionAsFieldName = true;
[Test]
        public void Property_ExportCaptionAsFieldName()
        {
            DataTable table;
            DataColumn column;
            table = new DataTable(&quot;Customers&quot;);

            //CustomerID column
            column = table.Columns.Add(&quot;CustomerID&quot;,

            System.Type.GetType(&quot;System.Int32&quot;));
            column.Unique = true;
            //CustomerName column
            column = table.Columns.Add(&quot;CustomerName&quot;,

            System.Type.GetType(&quot;System.String&quot;));
            column.Caption = &quot;Name&quot;;
            //CreditLimit
            column = table.Columns.Add(&quot;CreditLimit&quot;,

            System.Type.GetType(&quot;System.Double&quot;));
            column.DefaultValue = 0;
            column.Caption = &quot;Limit&quot;;
            table.Rows.Add(new object[] { 1, &quot;Jonathan&quot;, 23.44 });
            table.Rows.Add(new object[] { 2, &quot;Bill&quot;, 56.87 });

            var ExcelWorkBook = new Workbook();
            ExcelWorkBook.Worksheets.Add();
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.ExportCaptionAsFieldName = true;
            ExcelWorkBook.Worksheets[0].Cells.ImportData(table, 0, 0, options);
            Assert.AreEqual(&quot;Limit&quot;, ExcelWorkBook.Worksheets[0].Cells[&quot;C1&quot;].StringValue);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


