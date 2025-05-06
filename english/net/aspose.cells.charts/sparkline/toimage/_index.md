---
title: Sparkline.ToImage
second_title: Aspose.Cells for .NET API Reference
description: Sparkline method. Converts a sparkline to an image
type: docs
url: /net/aspose.cells.charts/sparkline/toimage/
---
## ToImage(ImageOrPrintOptions) {#toimage}

Converts a sparkline to an image.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The image options |

### Return Value

Returns a Bitmap object.

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_2}

Converts a sparkline to an image.

```csharp
public void ToImage(string fileName, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The image file name. |
| options | ImageOrPrintOptions | The image options |

### Examples

```csharp
// Called: line.ToImage(&amp;quot;output.png&amp;quot;, options);
public static void Method_ImageOrPrintOptions_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells[&quot;A1&quot;].PutValue(5);
            sheet.Cells[&quot;B1&quot;].PutValue(2);
            sheet.Cells[&quot;C1&quot;].PutValue(1);
            sheet.Cells[&quot;D1&quot;].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + &quot;!A1:D1&quot;, false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Add a sparkline to the group
            idx = group.Sparklines.Add(sheet.Name + &quot;!A1:D1&quot;, 0, 4);
            Sparkline line = group.Sparklines[idx];

            // Output sparkline details
            Console.WriteLine(&quot;Sparkline data range: &quot; + line.DataRange + &quot;, row: &quot; + line.Row + &quot;, column: &quot; + line.Column);

            // Save the sparkline as an image
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage(&quot;output.png&quot;, options);

            // Save the workbook
            workbook.Save(&quot;SparklineExample.xlsx&quot;);
        }
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_1}

Converts a sparkline to an image.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The image stream. |
| options | ImageOrPrintOptions | The image options. |

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


