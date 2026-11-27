---
title: "Sparkline.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Sparkline‑metod. Konverterar en sparkline till en bild"
type: docs
url: /sv/net/aspose.cells.charts/sparkline/toimage/
---
## ToImage(ImageOrPrintOptions) {#toimage}

Konverterar en sparkline till en bild.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | ImageOrPrintOptions | Bildalternativen |

### Returvärde

Returnerar ett Bitmap‑objekt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sparkline
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(15);
            sheet.Cells["D1"].PutValue(30);

            // Definiera platsen för sparkline
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            // Lägg till en sparkline‑grupp i kalkylbladet
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];
            Sparkline sparkline = group.Sparklines[0];

            try
            {
                // Skapa bildalternativ med realistiska inställningar
                ImageOrPrintOptions options = new ImageOrPrintOptions
                {
                    ImageType = Aspose.Cells.Drawing.ImageType.Jpeg,
                    HorizontalResolution = 200,
                    VerticalResolution = 200,
                    Quality = 90,
                    Transparent = false
                };

                // Spara sparkline till en fil med ToImage och ImageOrPrintOptions
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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_2}

Konverterar en sparkline till en bild.

```csharp
public void ToImage(string fileName, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Bildfilens namn. |
| alternativ | ImageOrPrintOptions | Bildalternativen |

### Exempel

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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_1}

Konverterar en sparkline till en bild.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Bildströmmen. |
| alternativ | ImageOrPrintOptions | Bildalternativen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiera CellArea för sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till en sparkline‑grupp i kalkylbladet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            Sparkline line = group.Sparklines[0];

            try
            {
                // Skapa en minnesström för att spara bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Skapa bildalternativ
                    ImageOrPrintOptions options = new ImageOrPrintOptions
                    {
                        ImageType = Aspose.Cells.Drawing.ImageType.Png,
                        HorizontalResolution = 300,
                        VerticalResolution = 300
                    };

                    // Anropa ToImage‑metoden med Stream och ImageOrPrintOptions
                    line.ToImage(stream, options);

                    // Spara strömmen till en fil
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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


