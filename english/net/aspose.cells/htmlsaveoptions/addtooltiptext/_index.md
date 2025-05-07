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
// Called: saveOptions.AddTooltipText = true;
[Test]
        public void Property_AddTooltipText()
        { 
            Workbook wb = new Aspose.Cells.Workbook(Constants.HtmlPath + "CELLSNET-55871.xlsx");
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);  
            saveOptions.AddTooltipText = true;
            wb.Save(_destFilesPath + "CELLSNET-55871.html", saveOptions);
            string text = File.ReadAllText(_destFilesPath + "CELLSNET-55871.html");
            Assert.IsTrue(text.IndexOf("style='overflow:hidden;' title='这是一段较长的文本数据，超出了单元格的宽度，转换到HTML文件后，依然无法显示或提示'>") >-1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


