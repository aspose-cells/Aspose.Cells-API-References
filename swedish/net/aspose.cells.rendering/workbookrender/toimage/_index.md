---
title: "WorkbookRender.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookRender-metod. Rendera hela arbetsboken som Tiff-bild till ström"
type: docs
url: /sv/net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

Rendera hela arbetsboken som Tiff-bild till en ström.

```csharp
public void ToImage(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | strömmen för den utgående bilden |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithStreamDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // Konfigurera bildrenderingsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // Skapa utdatamapp om den inte finns
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // Skapa en filström för bildutdata
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // Initiera arbetsboksgenererare och konvertera till bild
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // Spara den ursprungliga arbetsboken för referens
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### Se även

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

Rendera hela arbetsboken som Tiff-bild till en fil.

```csharp
public void ToImage(string filename)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | String | filnamnet för den utgående bilden |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // Ställ in bildalternativ
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // Skapa arbetsboksgenerering och spara till bild
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### Se även

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

Rendera en viss sida till en fil.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| fileName | String | filnamn för den utgående bilden |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Skapa bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // Skapa arbetsboksgenererare
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Spara varje sida som bild
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### Se även

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

Rendera en viss sida till en ström.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| ström | Ström | strömmen för den utgående bilden |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index and Stream Demo";

            // Konfigurera bildrenderingsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            try
            {
                // Initiera arbetsboksgenererare
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Hämta det första sidindexet (0-baserat)
                int pageIndex = 0;

                // Skapa en minnesström för att lagra bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Anropa ToImage med sidindex och ström
                    renderer.ToImage(pageIndex, stream);

                    // Visa resultat
                    Console.WriteLine($"Page {pageIndex} rendered successfully to stream");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");
                    Console.WriteLine($"Total pages available: {renderer.PageCount}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Rendera en viss sida till ett Bitmap-objekt.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |

### Returvärde

bitmap-objektet för sidan

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index Demo";

            // Konfigurera bildrenderingsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

            // Skapa utdatamapp om den inte finns
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            try
            {
                // Initiera arbetsboksgenererare
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Hämta det första sidindexet (0-baserat)
                int pageIndex = 0;

                // Anropa ToImage med sidindex och spara till fil
                string imagePath = Path.Combine(outputDir, $"page_{pageIndex}.png");
                renderer.ToImage(pageIndex, imagePath);

                Console.WriteLine($"Page {pageIndex} rendered successfully to: {imagePath}");
                Console.WriteLine($"Total pages available: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


