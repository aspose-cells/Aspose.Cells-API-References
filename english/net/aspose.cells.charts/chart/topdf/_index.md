---
title: Chart.ToPdf
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Saves the chart to a pdf file
type: docs
url: /net/aspose.cells.charts/chart/topdf/
---
## ToPdf(string) {#topdf_2}

Saves the chart to a pdf file.

```csharp
public void ToPdf(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the pdf file name with full path |

### Examples

```csharp
// Called: chart.ToPdf(Constants.destPath + &amp;quot;CELLSJAVA-4426_out.pdf&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-44268.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.ChartObject.IsHidden = (false);
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = (ImageType.Png);
            chart.ToImage(Constants.destPath + &quot;CELLSJAVA-4426_out.png&quot;, imgOptions);
            chart.ToPdf(Constants.destPath + &quot;CELLSJAVA-4426_out.pdf&quot;);

        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_3}

Saves the chart to a pdf file.

```csharp
public void ToPdf(string fileName, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the pdf file name with full path |
| desiredPageWidth | Single | The desired page width in inches. |
| desiredPageHeight | Single | The desired page height in inches. |
| hAlignmentType | PageLayoutAlignmentType | The chart horizontal alignment type in the output page. |
| vAlignmentType | PageLayoutAlignmentType | The chart vertical alignment type in the output page. |

### Examples

```csharp
// Called: chart.ToPdf(&amp;quot;ChartExample.pdf&amp;quot;, 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);
public static void Method_PageLayoutAlignmentType_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Sample Data&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(123);
            worksheet.Cells[&quot;A3&quot;].PutValue(456);
            worksheet.Cells[&quot;A4&quot;].PutValue(789);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Set the data range for the chart
            chart.SetChartDataRange(&quot;A1:A4&quot;, true);

            // Set the title of the chart
            chart.Title.Text = &quot;Sample Chart&quot;;

            // Save the workbook to a file
            workbook.Save(&quot;PageLayoutAlignmentTypeExample.xlsx&quot;);

            // Export the chart to a PDF with specific page layout alignment
            chart.ToPdf(&quot;ChartExample.pdf&quot;, 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
```

### See Also

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream) {#topdf}

Creates the chart pdf and saves it to a stream.

```csharp
public void ToPdf(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_1}

Creates the chart pdf and saves it to a stream.

```csharp
public void ToPdf(Stream stream, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| desiredPageWidth | Single | The desired page width in inches. |
| desiredPageHeight | Single | The desired page height in inches. |
| hAlignmentType | PageLayoutAlignmentType | The chart horizontal alignment type in the output page. |
| vAlignmentType | PageLayoutAlignmentType | The chart vertical alignment type in the output page. |

### See Also

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


