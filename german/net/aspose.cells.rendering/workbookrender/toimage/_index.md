---
title: "WorkbookRender.ToImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookRender-Methode. Gesamte Arbeitsmappe als Tiff-Bild in einen Stream rendern"
type: docs
url: /de/net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

Rendert die gesamte Arbeitsmappe als TIFF-Bild in einen Stream.

```csharp
public void ToImage(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | der Stream des Ausgabebildes |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // Konfigurieren Sie die Bildrenderoptionen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // Erstelle Ausgabeverzeichnis, falls es nicht existiert
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // Dateistream für die Bildausgabe erstellen
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // Arbeitsmappen-Renderer initialisieren und in ein Bild konvertieren
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // Die ursprüngliche Arbeitsmappe zur Referenz speichern
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### Siehe auch

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

Rendert die gesamte Arbeitsmappe als TIFF-Bild in eine Datei.

```csharp
public void ToImage(string filename)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateiname | String | der Dateiname des Ausgabebildes |

### Beispiele

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
            // Erstelle ein Beispielarbeitsbuch
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // Lege Bildoptionen fest
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // Arbeitsmappen-Render erstellen und als Bild speichern
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

Rendert eine bestimmte Seite in eine Datei.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| fileName | String | Dateiname des Ausgabebildes |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Bildoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // Arbeitsmappen-Renderer erstellen
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Jede Seite als Bild speichern
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### Siehe auch

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

Rendert eine bestimmte Seite in einen Stream.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| Stream | Stream | der Stream des Ausgabebildes |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index and Stream Demo";

            // Konfigurieren Sie die Bildrenderoptionen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            try
            {
                // Arbeitsmappen-Renderer initialisieren
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Den ersten Seitenindex (0-basiert) erhalten
                int pageIndex = 0;

                // Memory-Stream erstellen, um das Bild zu halten
                using (MemoryStream stream = new MemoryStream())
                {
                    // ToImage mit Seitenindex und Stream aufrufen
                    renderer.ToImage(pageIndex, stream);

                    // Ergebnisse anzeigen
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

### Siehe auch

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Rendert eine bestimmte Seite in ein Bitmap-Objekt.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |

### Rückgabewert

das Bitmap-Objekt der Seite

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index Demo";

            // Konfigurieren Sie die Bildrenderoptionen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

            // Erstelle Ausgabeverzeichnis, falls es nicht existiert
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            try
            {
                // Arbeitsmappen-Renderer initialisieren
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Den ersten Seitenindex (0-basiert) erhalten
                int pageIndex = 0;

                // Rufen Sie ToImage mit Seitenindex auf und speichern Sie in eine Datei
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

### Siehe auch

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


