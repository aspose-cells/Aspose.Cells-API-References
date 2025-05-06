---
title: HtmlSaveOptions.IsExportComments
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if exporting comments when saving file to html the default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Indicates if exporting comments when saving file to html, the default value is false.

```csharp
public bool IsExportComments { get; set; }
```

### Examples

```csharp
// Called: options.IsExportComments = false;
[Test]
        public void Property_IsExportComments()
        {
          
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;NET47864.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;
            options.ExcludeUnusedStyles = true;
            options.IsExportComments = false;
            options.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            options.ExportBogusRowData = true;
            options.ExportFrameScriptsAndProperties = false;
            options.WidthScalable = false;
            options.ExportHeadings = true;
            workbook.Save(Constants.destPath + &quot;NET47864.html&quot;, options);
            workbook = new Workbook(Constants.destPath + &quot;NET47864.html&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(&quot;6&quot;, cells[&quot;A7&quot;].StringValue);
            Assert.IsTrue(cells.IsRowHidden(6));
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


