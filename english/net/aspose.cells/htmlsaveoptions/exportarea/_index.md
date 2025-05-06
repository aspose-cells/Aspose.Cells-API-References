---
title: HtmlSaveOptions.ExportArea
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.

```csharp
public CellArea ExportArea { get; set; }
```

### Examples

```csharp
// Called: ExportArea = CellArea.CreateCellArea(&amp;quot;A1&amp;quot;, &amp;quot;C6&amp;quot;),
[Test]
        public void Property_ExportArea()
        {
            using (var wb = new Workbook(Constants.HtmlSourcePath + &quot;CellsNet52181.xlsx&quot;))
            {
                var options = new HtmlSaveOptions(SaveFormat.Html)
                {
                    Encoding = Encoding.UTF8,
                    ExportActiveWorksheetOnly = true,

                    ExportArea = CellArea.CreateCellArea(&quot;A1&quot;, &quot;C6&quot;),
                };


                wb.Save(Constants.HtmlDestPath + &quot;CellsNet52181.html&quot;, options);
                string text = File.ReadAllText(Constants.HtmlDestPath + &quot;CellsNet52181.html&quot;);
                Assert.IsTrue(text.IndexOf(&quot;&lt;table class=&apos;x21&apos;&quot;) != -1);
            }
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


