---
title: "Chart.ToPdf"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Methode. Speichert das Diagramm in einer PDF‑Datei"
type: docs
url: /de/net/aspose.cells.charts/chart/topdf/
---
## ToPdf(string) {#topdf_2}

Speichert das Diagramm in einer PDF-Datei.

```csharp
public void ToPdf(string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der PDF‑Dateiname mit vollständigem Pfad |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Diagramm nach PDF exportieren
            chart.ToPdf("output_chart.pdf");
            
            Console.WriteLine("Chart exported to PDF successfully.");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_3}

Speichert das Diagramm in einer PDF-Datei.

```csharp
public void ToPdf(string fileName, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der PDF‑Dateiname mit vollständigem Pfad |
| desiredPageWidth | Einzeln | Die gewünschte Seitenbreite in Zoll. |
| desiredPageHeight | Einzeln | Die gewünschte Seitenhöhe in Zoll. |
| hAlignmentType | PageLayoutAlignmentType | Der horizontale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |
| vAlignmentType | PageLayoutAlignmentType | Der vertikale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |

### Beispiele

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

### Siehe auch

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream) {#topdf}

Erstellt das Diagramm-PDF und speichert es in einen Stream.

```csharp
public void ToPdf(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Ausgabestream. |

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm einfügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(45);
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B4"].PutValue(25);

            // Füge ein Säulendiagramm zum Arbeitsblatt hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Setzt die Datenquelle für das Diagramm
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Exportieren Sie das Diagramm in ein PDF mithilfe eines FileStreams
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

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_1}

Erstellt das Diagramm-PDF und speichert es in einen Stream.

```csharp
public void ToPdf(Stream stream, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Ausgabestream. |
| desiredPageWidth | Einzeln | Die gewünschte Seitenbreite in Zoll. |
| desiredPageHeight | Einzeln | Die gewünschte Seitenhöhe in Zoll. |
| hAlignmentType | PageLayoutAlignmentType | Der horizontale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |
| vAlignmentType | PageLayoutAlignmentType | Der vertikale Ausrichtungstyp des Diagramms auf der Ausgabeseite. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Erstellen Sie einen Memory-Stream, um das PDF zu speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    // Rufen Sie die Methode ToPdf mit den Parametern Stream, Single, Single, PageLayoutAlignmentType, PageLayoutAlignmentType auf
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

            // Speichere die Arbeitsmappe
            workbook.Save("ChartToPdfDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


