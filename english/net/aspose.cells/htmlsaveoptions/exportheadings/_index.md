---
title: HtmlSaveOptions.ExportHeadings
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exports sheets row and column headings when saving to HTML files
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Indicates whether exports sheet's row and column headings when saving to HTML files.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: options.ExportHeadings = true;
[Test]
        public void Property_ExportHeadings()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47030/&quot;;

            string savePath = CreateFolder(filePath);
            Workbook wb = new Workbook(filePath + &quot;a.xlsx&quot;);

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;
            wb.Save(savePath + &quot;a_out.html&quot;, options);

            wb = new Workbook(filePath + &quot;input.xls&quot;);
            wb.Save(savePath + &quot;sample_out.html&quot;, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


