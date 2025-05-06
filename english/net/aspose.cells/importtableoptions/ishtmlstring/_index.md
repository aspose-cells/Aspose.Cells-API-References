---
title: ImportTableOptions.IsHtmlString
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether the value contains html tags
type: docs
url: /net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Indicates whether the value contains html tags.

```csharp
public bool IsHtmlString { get; set; }
```

### Examples

```csharp
// Called: IsHtmlString = true
[Test]
        public void Property_IsHtmlString()
        {
            DataTable table = new DataTable();
            table.Columns.Add(&quot;ID&quot;);
            table.Columns.Add(&quot;thelink&quot;);
            table.Columns.Add(&quot;Start Time&quot;);
            string[] addrow = { &quot;1&quot;, &quot;&lt;p&gt;&lt;a href=\&quot;https://reactjs.org/blog/2018/09/10/introducing-the-react-profiler.html\&quot;&gt;CN Risk 3&lt;/a&gt;&amp;nbsp;&lt;/p&gt;&quot;, &quot;1:00 PM&quot; };
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
            Assert.AreEqual(ws.Hyperlinks.Count, 1);
            workbook.Save(Constants.destPath + &quot;CELLSNET50380.xlsx&quot;);

        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


