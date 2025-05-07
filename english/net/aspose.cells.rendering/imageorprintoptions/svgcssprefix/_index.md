---
title: ImageOrPrintOptions.SvgCssPrefix
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets and sets the prefix of the css name in svgthe default value is empty string
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/svgcssprefix/
---
## ImageOrPrintOptions.SvgCssPrefix property

Gets and sets the prefix of the css name in svg,the default value is empty string.

```csharp
[Obsolete("Use SvgImageOptions.CssPrefix property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SvgCssPrefix { get; set; }
```

### Examples

```csharp
// Called: imgOpt.SvgCssPrefix = prefix;
[Test]
        public void Property_SvgCssPrefix()
        {
            string prefix = "x_";

            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Svg css prefix");

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Svg;
            imgOpt.OnePagePerSheet = true;
            imgOpt.SvgCssPrefix = prefix;

            SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);
            using(MemoryStream ms = new MemoryStream())
            {
                sr.ToImage(0, ms);
                ms.Position = 0;
                using(StreamReader reader = new StreamReader(ms))
                {
                    string content = reader.ReadToEnd();
                    Assert.IsTrue(content.IndexOf(prefix + "f") > -1, "Svg css prefix doesn't work.");
                }
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


