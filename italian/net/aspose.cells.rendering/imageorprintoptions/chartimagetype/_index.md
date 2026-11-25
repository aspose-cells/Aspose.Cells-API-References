---
title: "ImageOrPrintOptions.ChartImageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Indica il tipo di immagine del grafico durante la conversione. valore predefinito PNG"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/chartimagetype/
---
## ImageOrPrintOptions.ChartImageType property

Indica il tipo di immagine del grafico durante la conversione. valore predefinito: PNG.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ChartImageType { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, Chart e Shape vengono sempre renderizzati come elementi vettoriali (ad es. punto, linea) per la qualità del rendering. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyChartImageTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un worksheet con un grafico
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:A4", true);

            try
            {
                // Crea un'istanza di ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visualizza il valore corrente di ChartImageType
                Console.WriteLine("Current ChartImageType: " + options.ImageType);

                // Imposta un tipo di immagine diverso per il rendering del grafico
                options.ImageType = ImageType.Png;
                Console.WriteLine("ChartImageType set to: " + options.ImageType);

                // Crea un SheetRender per dimostrare l'effetto della proprietà
                SheetRender renderer = new SheetRender(worksheet, options);

                // Renderizza il grafico in uno stream di memoria
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Chart rendered successfully with ChartImageType: " + options.ImageType);
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Salva la cartella di lavoro
                workbook.Save("ChartImageTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


