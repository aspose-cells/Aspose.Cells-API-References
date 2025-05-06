---
title: Range.ToImage
second_title: Aspose.Cells for .NET API Reference
description: Range method. Converts the range to image
type: docs
url: /net/aspose.cells/range/toimage/
---
## Range.ToImage method

Converts the range to image.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The options for converting this range to image |

### Examples

```csharp
// Called: byte[] data = r.ToImage(null);
[Test]
        public void Method_ImageOrPrintOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET55578.xlsx&quot;);
            //A1:J25
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range r = cells.CreateRange(&quot;A1:J25&quot;);
            byte[] data = r.ToImage(null);

            byte[] htmlData = r.ToHtml(null);
            string json = r.ToJson(null);
        }
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


