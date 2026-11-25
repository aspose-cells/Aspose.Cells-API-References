---
title: "Sparkline.ToImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Sparkline. Converte uno sparkline in un'immagine"
type: docs
url: /it/net/aspose.cells.charts/sparkline/toimage/
---
## ToImage(ImageOrPrintOptions) {#toimage}

Converte uno sparkline in un'immagine.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | ImageOrPrintOptions | Le opzioni dell'immagine |

### Valore di ritorno

Restituisce un oggetto Bitmap.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithImageOrPrintOptDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per lo sparkline
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(15);
            sheet.Cells["D1"].PutValue(30);

            // Definisci la posizione per lo sparkline
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            // Aggiungi un gruppo di sparkline al foglio di lavoro
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];
            Sparkline sparkline = group.Sparklines[0];

            try
            {
                // Crea opzioni immagine con impostazioni realistiche
                ImageOrPrintOptions options = new ImageOrPrintOptions
                {
                    ImageType = Aspose.Cells.Drawing.ImageType.Jpeg,
                    HorizontalResolution = 200,
                    VerticalResolution = 200,
                    Quality = 90,
                    Transparent = false
                };

                // Salva lo sparkline in un file usando ToImage con ImageOrPrintOptions
                sparkline.ToImage("sparkline_demo.jpg", options);

                Console.WriteLine("Sparkline successfully saved as image with custom options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving sparkline as image: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_2}

Converte uno sparkline in un'immagine.

```csharp
public void ToImage(string fileName, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome del file immagine. |
| opzioni | ImageOrPrintOptions | Le opzioni dell'immagine |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SparklineMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            Sparkline line = group.Sparklines[0];

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            line.ToImage("sparkline_output.png", options);
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_1}

Converte uno sparkline in un'immagine.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso dell'immagine. |
| opzioni | ImageOrPrintOptions | Le opzioni dell'immagine. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithStreamImageOrPrintOptDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definisci il CellArea per lo sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo di sparkline al foglio di lavoro
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            Sparkline line = group.Sparklines[0];

            try
            {
                // Crea un flusso di memoria per salvare l'immagine
                using (MemoryStream stream = new MemoryStream())
                {
                    // Crea opzioni immagine
                    ImageOrPrintOptions options = new ImageOrPrintOptions
                    {
                        ImageType = Aspose.Cells.Drawing.ImageType.Png,
                        HorizontalResolution = 300,
                        VerticalResolution = 300
                    };

                    // Chiama il metodo ToImage con Stream e ImageOrPrintOptions
                    line.ToImage(stream, options);

                    // Salva il flusso in un file
                    File.WriteAllBytes("sparkline_stream_output.png", stream.ToArray());
                    Console.WriteLine("Sparkline image saved successfully using stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToImage: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


