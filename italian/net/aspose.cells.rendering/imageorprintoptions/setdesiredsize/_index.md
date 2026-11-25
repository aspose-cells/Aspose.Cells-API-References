---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ImageOrPrintOptions. Imposta la larghezza e l'altezza desiderate dell'immagine"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Imposta la larghezza e l'altezza desiderate dell'immagine.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| desiredWidth | Int32 | larghezza desiderata in pixel |
| desiredHeight | Int32 | altezza desiderata in pixel |

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare `SetDesiredSize` impostando il parametro keepAspectRatio a false. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Imposta l'area di stampa
            worksheet.PageSetup.PrintArea = "A1:A11";

            // Crea opzioni immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Renderizza il foglio di lavoro in immagine
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Imposta la larghezza e l'altezza desiderate dell'immagine.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| desiredWidth | Int32 | larghezza desiderata in pixel |
| desiredHeight | Int32 | altezza desiderata in pixel |
| keepAspectRatio | Booleano | se mantenere il rapporto d'aspetto dell'immagine originale |

### Osservazioni

La larghezza e l'altezza dell'immagine di output in pixel saranno basate esclusivamente sulla larghezza e altezza desiderate impostate.

Le [`HorizontalResolution`](../horizontalresolution/) e le [`VerticalResolution`](../verticalresolution/) non influenzeranno la larghezza e l'altezza dell'immagine di output in questo caso.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e crea un grafico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Ottieni la forma del grafico
            Shape chartShape = worksheet.Shapes[0];

            // Imposta le opzioni dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // Salva il grafico come immagine
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // Salva l'immagine su file
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


