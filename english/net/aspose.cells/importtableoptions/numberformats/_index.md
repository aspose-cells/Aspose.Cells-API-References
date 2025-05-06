---
title: ImportTableOptions.NumberFormats
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets the number formats
type: docs
url: /net/aspose.cells/importtableoptions/numberformats/
---
## ImportTableOptions.NumberFormats property

Gets or sets the number formats

```csharp
public string[] NumberFormats { get; set; }
```

### Examples

```csharp
// Called: NumberFormats = new string[] { null, null, &amp;quot;h:mm AM/PM&amp;quot; },
[Test]
        public void Property_NumberFormats()
        {
            System.Data.DataTable table = new System.Data.DataTable();
            table.Columns.Add(&quot;ID&quot;);
            table.Columns.Add(&quot;thelink&quot;);
            table.Columns.Add(&quot;Start Time&quot;);
            string[] addrow = { &quot;1&quot;, &quot;&lt;span style=&apos;width: 240px; overflow: hidden; white-space: nowrap; display: inline-block; text-overflow:ellipsis;&apos;&gt;&lt;a href=&apos;http://mysite.com/includes/pdfcrowd/pdfAPI.php?url=https%3A%2F%2Fwww%2mysite%2Ecom%2Fcfp2%2FReviews%2FTools%2FPreview%2Dall%2Easp%3FEventID%3D9638%26ClientID%3D2465%26SubID%3D716990&amp;pageheight=11in&apos; target=&apos;_blank&apos;&gt;Submission Preview&lt;/a&gt;&lt;/span&gt;&quot;, &quot;1:00 PM&quot; };
            table.Rows.Add(addrow);

            var workbook = new Workbook();
            var ws = workbook.Worksheets[0];
            ws.Cells.ImportData(table, 0, 0, new ImportTableOptions
            {
                IsFieldNameShown = true,
                ConvertNumericData = true,
                NumberFormats = new string[] { null, null, &quot;h:mm AM/PM&quot; },
                IsHtmlString = true


            });
            Hyperlink link = workbook.Worksheets[0].Hyperlinks[0];
            Assert.AreEqual(1, link.Area.StartRow);
            Assert.AreEqual(1, link.Area.StartColumn);
            workbook.Save(_destFilesPath + &quot;CellsNet46904.xlsx&quot;);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


