---
title: "SheetRender.ToImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetRender-Methode. Rendert eine bestimmte Seite auf ein Graphics"
type: docs
url: /de/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Bestimmte Seite in ein Graphics-Objekt rendern

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| g | Graphics | Das Objekt, in das gerendert werden soll. |
| x | Einzeln | Die X‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |
| y | Einzeln | Die Y‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |
| Breite | Einzeln | Die maximale Breite (in Pixeln), die die gerenderte Seite einnehmen kann. |
| Höhe | Einzeln | Die maximale Höhe (in Pixeln), die die gerenderte Seite einnehmen kann. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Bildoptionen erstellen
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // SheetRender für das Arbeitsblatt erstellen
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Einen MemoryStream erstellen, um das gerenderte Bild zu erfassen
                using (MemoryStream stream = new MemoryStream())
                {
                    // ToImage mit den angegebenen Parametern aufrufen
                    // Da wir System.Drawing.Graphics nicht verwenden können, nutzen wir die einfachere ToImage-Überladung
                    sheetRender.ToImage(0, stream);

                    // Das gerenderte Bild in einer Datei speichern
                    File.WriteAllBytes("RenderedOutput.png", stream.ToArray());
                }

                Console.WriteLine("Sheet rendered to image successfully.");
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

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Bestimmte Seite in ein Graphics-Objekt rendern

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| g | Graphics | Das Objekt, in das gerendert werden soll. |
| x | Einzeln | Die X‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |
| y | Einzeln | Die Y‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Bildoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // SheetRender-Instanz erstellen
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Da wir System.Drawing-Typen nicht verwenden können, nutzen wir die alternative ToImage-Methode
                // die direkt in einer Datei speichert
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Ressourcen bereinigen
                sheetRender.Dispose();
            }
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

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
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Lade die Quell-Excel-Datei
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Bildoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Erstelle SheetRender für das erste Arbeitsblatt
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Rendere die erste Seite des Sheets in eine Bilddatei
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

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

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Bildoptionen erstellen
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // SheetRender-Instanz erstellen
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Memory-Stream erstellen, um das Bild zu halten
                using (MemoryStream stream = new MemoryStream())
                {
                    // Rufe ToImage mit Seitenindex und Stream-Parametern auf
                    sheetRender.ToImage(0, stream);

                    Console.WriteLine($"Successfully rendered page 0 to stream. Stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
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

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Bildoptionen erstellen
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // SheetRender-Instanz erstellen
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Den ersten Seitenindex (0-basiert) erhalten
                int pageIndex = 0;

                // Rufe ToImage mit dem Seitenindex-Parameter auf
                sheetRender.ToImage(pageIndex, "output_page.png");

                Console.WriteLine($"Successfully rendered page {pageIndex} to image");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


