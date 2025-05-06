---
title: HtmlSaveOptions.AddTooltipText
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether adding tooltip text when the data cant be fully displayed. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/addtooltiptext/
---
## HtmlSaveOptions.AddTooltipText property

Indicates whether adding tooltip text when the data can't be fully displayed. The default value is false.

```csharp
public bool AddTooltipText { get; set; }
```

### Examples

```csharp
// Called: options.AddTooltipText = true;
[Test]
        public void Property_AddTooltipText()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA43047/&quot;;

            string savePath = CreateFolder(filePath);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.AddTooltipText = true;
            Workbook wb = new Workbook(filePath + &quot;test1.xls&quot;);
            wb.Save(savePath + &quot;test1_out.html&quot;, options);

            wb = new Workbook(filePath + &quot;a.xlsx&quot;);
            wb.Save(savePath + &quot;a_out.html&quot;, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


