---
title: "Chart.ToPdf"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Salva il grafico in un file pdf"
type: docs
url: /it/net/aspose.cells.charts/chart/topdf/
---
## ToPdf(string) {#topdf_2}

Salva il grafico in un file PDF.

```csharp
public void ToPdf(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | il nome del file pdf con percorso completo |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Esporta il grafico in PDF
            chart.ToPdf("output_chart.pdf");
            
            Console.WriteLine("Chart exported to PDF successfully.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_3}

Salva il grafico in un file PDF.

```csharp
public void ToPdf(string fileName, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | il nome del file pdf con percorso completo |
| desiredPageWidth | Single | La larghezza desiderata della pagina in pollici. |
| desiredPageHeight | Single | L'altezza desiderata della pagina in pollici. |
| hAlignmentType | PageLayoutAlignmentType | Il tipo di allineamento orizzontale del grafico nella pagina di output. |
| vAlignmentType | PageLayoutAlignmentType | Il tipo di allineamento verticale del grafico nella pagina di output. |

### Esempi

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

### Vedi anche

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream) {#topdf}

Crea il PDF del grafico e lo salva in uno stream.

```csharp
public void ToPdf(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |

### Esempi

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
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(45);
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B4"].PutValue(25);

            // Aggiungi un grafico a colonne al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'origine dati per il grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Esporta il grafico in PDF usando un FileStream
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

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToPdf(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) {#topdf_1}

Crea il PDF del grafico e lo salva in uno stream.

```csharp
public void ToPdf(Stream stream, float desiredPageWidth, float desiredPageHeight, 
    PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di output. |
| desiredPageWidth | Single | La larghezza desiderata della pagina in pollici. |
| desiredPageHeight | Single | L'altezza desiderata della pagina in pollici. |
| hAlignmentType | PageLayoutAlignmentType | Il tipo di allineamento orizzontale del grafico nella pagina di output. |
| vAlignmentType | PageLayoutAlignmentType | Il tipo di allineamento verticale del grafico nella pagina di output. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Crea uno stream di memoria per salvare il PDF
                using (MemoryStream stream = new MemoryStream())
                {
                    // Chiama il metodo ToPdf con i parametri Stream, Single, Single, PageLayoutAlignmentType, PageLayoutAlignmentType
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

            // Salva la cartella di lavoro
            workbook.Save("ChartToPdfDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PageLayoutAlignmentType](../../../aspose.cells/pagelayoutalignmenttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


