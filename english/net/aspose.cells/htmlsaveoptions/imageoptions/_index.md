---
title: HtmlSaveOptions.ImageOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Get the ImageOrPrintOptions object before exporting
type: docs
url: /net/aspose.cells/htmlsaveoptions/imageoptions/
---
## HtmlSaveOptions.ImageOptions property

Get the ImageOrPrintOptions object before exporting

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Examples

```csharp
// Called: options2.ImageOptions.ImageType = ImageType.Svg;
[Test]
        public void Property_ImageOptions()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET48003/&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = null;
            wb = new Workbook(filePath + &quot;getCarSVG.html&quot;);
            wb.Save(savePath + &quot;Car_out.xlsx&quot;);

            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            options.AutoFitColsAndRows = true;
            wb = new Workbook(filePath + &quot;Summer Bra – Shop Calltv.mhtml&quot;, options);
            wb.Save(savePath + &quot;SummerBra_out.xlsx&quot;);

            wb = new Workbook(filePath + &quot;SummerBra_out.xlsx&quot;);
            HtmlSaveOptions options2 = new HtmlSaveOptions();
            options2.ImageOptions.ImageType = ImageType.Svg;
            wb.Save(savePath + &quot;out.html&quot;, options2);
        }
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


