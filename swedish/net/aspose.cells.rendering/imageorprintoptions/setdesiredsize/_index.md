---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-metoden. Anger önskad bredd och höjd för bilden."
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Anger önskad bredd och höjd på bilden.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredWidth | Int32 | önskad bredd i pixlar |
| desiredHeight | Int32 | önskad höjd i pixlar |

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället `SetDesiredSize` genom att sätta parametern keepAspectRatio till false. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Ställ in utskriftsområde
            worksheet.PageSetup.PrintArea = "A1:A11";

            // Skapa bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Rendera kalkylblad till bild
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Anger önskad bredd och höjd på bilden.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredWidth | Int32 | önskad bredd i pixlar |
| desiredHeight | Int32 | önskad höjd i pixlar |
| keepAspectRatio | Boolean | om bildens ursprungliga bildförhållande ska behållas |

### Anmärkningar

Bredden och höjden på utdata bilden i pixlar kommer endast att baseras på den angivna önskade bredden och höjden.

[`HorizontalResolution`](../horizontalresolution/) och [`VerticalResolution`](../verticalresolution/) kommer inte att påverka bredden och höjden på utdata bilden i detta fall.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och skapa ett diagram
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

            // Hämta diagrammets form
            Shape chartShape = worksheet.Shapes[0];

            // Ställ in bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // Spara diagrammet som bild
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // Spara bilden till fil
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


