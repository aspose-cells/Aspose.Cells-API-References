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
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToPdfWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet and add sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data source
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Export chart to PDF
            chart.ToPdf("output_chart.pdf");
            
            Console.WriteLine("Chart exported to PDF successfully.");
        }
    }
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
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToPdfWithStringSingleSinglePageLayoutAlDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:A4", true);
            chart.Title.Text = "Demo Chart";

            chart.ToPdf("ChartDemo.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);
        }
    }
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

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToPdfWithStreamDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(32);
            worksheet.Cells["B4"].PutValue(23);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Set chart data range
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Create a memory stream to save the PDF
                using (MemoryStream pdfStream = new MemoryStream())
                {
                    // Call the ToPdf method with Stream parameter
                    chart.ToPdf(pdfStream);

                    // Save the stream to a file for demonstration
                    File.WriteAllBytes("ChartToPdfStreamOutput.pdf", pdfStream.ToArray());
                }

                Console.WriteLine("Chart successfully converted to PDF using Stream parameter.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToPdf method: {ex.Message}");
            }
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToPdfWithStreamSingleSinglePageLayoutAlDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Set chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Create a memory stream to save the PDF
            using (MemoryStream pdfStream = new MemoryStream())
            {
                try
                {
                    // Call ToPdf with specific parameters
                    chart.ToPdf(
                        pdfStream, 
                        800f, // desiredPageWidth
                        600f, // desiredPageHeight
                        PageLayoutAlignmentType.Center, // horizontal alignment
                        PageLayoutAlignmentType.Center // vertical alignment
                    );

                    Console.WriteLine("Chart successfully converted to PDF with specified layout parameters.");
                    
                    // Save the PDF stream to a file for demonstration
                    File.WriteAllBytes("ChartToPdfWithLayout.pdf", pdfStream.ToArray());
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error converting chart to PDF: {ex.Message}");
                }
            }

            // Save the workbook
            workbook.Save("ChartMethodToPdfDemo.xlsx");
        }
    }
}
```

### See Also

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


