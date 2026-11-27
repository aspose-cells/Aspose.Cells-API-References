---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageSaveOptions‑konstruktör. Skapar alternativen för att spara bildfil"
type: docs
url: /sv/net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

Skapar alternativen för att spara bildfil.

```csharp
public ImageSaveOptions()
```

### Anmärkningar

Standardtypen är Tiff.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ImageSaveOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Visa den parameterlösa konstruktorn
                ImageSaveOptions defaultOptions = new ImageSaveOptions();
                Console.WriteLine("Created ImageSaveOptions with default constructor");

                // Visa konstruktorn med SaveFormat‑parameter
                ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
                Console.WriteLine("Created ImageSaveOptions with SaveFormat.Png");

                // Kom åt den skrivskyddade ImageOrPrintOptions‑egenskapen
                var imageOptions = pngOptions.ImageOrPrintOptions;
                Console.WriteLine($"ImageOrPrintOptions type: {imageOptions.GetType().Name}");

                // Ange StreamProvider‑egenskapen
                pngOptions.StreamProvider = null;
                Console.WriteLine("StreamProvider set to null");

                // Spara arbetsboken med de skapade alternativen
                workbook.Save("output.png", pngOptions);
                Console.WriteLine("Workbook saved successfully with ImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativen för att spara bildfil.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Filformatet. Det bör vara en av följande typer: Tiff, Svg, Bmp, Png, Jpg, Emf eller Gif, annars kommer det sparade formatet automatiskt att sättas till Tiff. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och lägg till testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
            
            // Skapa ImageSaveOptions med SaveFormat.Tiff
            try
            {
                ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
                
                // Konfigurera bildrenderingsalternativ
                saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
                saveOptions.ImageOrPrintOptions.VerticalResolution = 300;

                // Spara arbetsboken som flersidig TIFF
                workbook.Save("WorksheetImage.tiff", saveOptions);
                
                Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image save operation: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


