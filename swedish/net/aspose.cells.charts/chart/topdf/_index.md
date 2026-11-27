---
title: "Chart.ToPdf"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagrammetod. Sparar diagrammet till en pdf-fil"
type: docs
url: /sv/net/aspose.cells.charts/chart/topdf/
---
## ToPdf(string) {#topdf_2}

Sparar diagrammet till en pdf-fil.

```csharp
public void ToPdf(string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | pdf-filnamnet med fullständig sökväg |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Exportera diagram till PDF
            chart.ToPdf("output_chart.pdf");
            
            Console.WriteLine("Chart exported to PDF successfully.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_3}

Sparar diagrammet till en pdf-fil.

```csharp
public void ToPdf(string fileName, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | pdf-filnamnet med fullständig sökväg |
| desiredPageWidth | Single | Den önskade sidbredden i tum. |
| desiredPageHeight | Single | Den önskade sidhöjden i tum. |
| hAlignmentType | PageLayoutAlignmentType | Diagrammets horisontella justeringstyp på utskriftssidan. |
| vAlignmentType | PageLayoutAlignmentType | Diagrammets vertikala justeringstyp på utskriftssidan. |

### Exempel

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

### Se även

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream) {#topdf}

Skapar diagrammets PDF och sparar den till en ström.

```csharp
public void ToPdf(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToPdfWithStreamDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(45);
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B4"].PutValue(25);

            // Lägg till ett stapeldiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange datakällan för diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Exportera diagrammet till en PDF med en FileStream
                using (FileStream pdfStream = new FileStream("ChartOutput.pdf", FileMode.Create, FileAccess.Write))
                {
                    chart.ToPdf(pdfStream);
                }

                Console.WriteLine("Chart successfully exported to ChartOutput.pdf");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting chart to PDF: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_1}

Skapar diagrammets pdf och sparar den till en ström.

```csharp
public void ToPdf(Stream stream, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen. |
| desiredPageWidth | Single | Den önskade sidbredden i tum. |
| desiredPageHeight | Single | Den önskade sidhöjden i tum. |
| hAlignmentType | PageLayoutAlignmentType | Diagrammets horisontella justeringstyp på utskriftssidan. |
| vAlignmentType | PageLayoutAlignmentType | Diagrammets vertikala justeringstyp på utskriftssidan. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToPdfWithStreamSingleSinglePageLayoutAl115534Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Skapa en minnesström för att spara PDF-filen
                using (MemoryStream stream = new MemoryStream())
                {
                    // Anropa metoden ToPdf med parametrarna Stream, Single, Single, PageLayoutAlignmentType, PageLayoutAlignmentType
                    float desiredPageWidth = 8.5f; // 8.5 inches
                    float desiredPageHeight = 11f; // 11 inches
                    PageLayoutAlignmentType hAlignment = PageLayoutAlignmentType.Center;
                    PageLayoutAlignmentType vAlignment = PageLayoutAlignmentType.Center;

                    chart.ToPdf(stream, desiredPageWidth, desiredPageHeight, hAlignment, vAlignment);

                    Console.WriteLine("Chart successfully converted to PDF in memory stream.");
                    Console.WriteLine($"PDF stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to PDF: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("ChartToPdfDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


