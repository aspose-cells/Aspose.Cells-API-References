---
title: "Chart.ToImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Methode. Gibt ein 32‑Bit‑Bitmap‑Objekt des Diagramms zurück"
type: docs
url: /de/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Ermittelt ein 32‑Bit `Bitmap`‑Objekt des Diagramms.

```csharp
public Bitmap ToImage()
```

### Rückgabewert

das Bild des Diagramms.

### Hinweise

Wenn Breite oder Höhe null ist oder das Diagramm laut unterstützter Diagrammliste nicht unterstützt wird, gibt es null zurück.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:B4", true);
            
            // Diagramm in Bild konvertieren und in Datei speichern
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Ermittelt ein 32‑Bit `Bitmap`‑Objekt des Diagramms. Die Attribute `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression und ImageOrPrintOptions.Quality werden ignoriert.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | ImageOrPrintOptions | Zusätzliche Optionen zur Bildgenerierung |

### Rückgabewert

das Bild des Diagramms.

### Hinweise

Gibt ein 32‑Bit‑Bitmap‑Objekt zurück, sodass die Attribute ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression und ImageOrPrintOptions.Quality die Methode nicht beeinflussen. Wenn Breite oder Höhe null ist oder das Diagramm laut unterstützter Diagrammliste nicht unterstützt wird, gibt es null zurück.

### Beispiele

Gibt ein Bitmap‑Objekt mit 200 dpi in x‑Richtung und 300 dpi in y‑Richtung zurück.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 200;
options.VerticalResolution = 300;

Workbook book = new Workbook(@"test.xls");
Bitmap chartObject = book.Worksheets[0].Charts[0].ToImage(options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 200
options.VerticalResolution = 300

Dim book As Workbook =  New Workbook("test.xls")
Dim chartObject As Bitmap = book.Worksheets(0).Charts(0).ToImage(options)

```

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Bildformat.

```csharp
public void ToImage(string imageFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |

### Hinweise

Das Format des Bildes wird anhand der Dateierweiterung festgelegt. Beispiel: Wenn Sie "myfile.png" angeben, wird das Bild im PNG‑Format gespeichert. Die folgenden Dateierweiterungen werden erkannt: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Wenn Breite oder Höhe null ist oder das Diagramm laut unterstützter Diagrammliste nicht unterstützt wird, führt diese Methode nichts aus.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Diagramm als Bild speichern
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Format.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |
| imageFormat | ImageFormat | Das Format, in dem das Bild gespeichert werden soll. |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Chart.ToImage(string, ImageType). Diese Eigenschaft wird 12 Monate nach Juli 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |
| imageType | ImageType | Der Bildtyp, in dem das Bild gespeichert werden soll. |

### Hinweise

Der Bildtyp wird über `imageType` festgelegt. Die folgenden Typen werden unterstützt: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Wenn Breite oder Höhe null ist oder das Diagramm laut unterstützter Diagrammliste nicht unterstützt wird, führt diese Methode nichts aus.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm mit angegebenem ImageType als Bild speichern
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### Siehe auch

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Erstellt das Diagrammbild und speichert es in einer Datei im Jpeg-Format.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |
| jpegQuality | Int64 | Jpeg-Qualität. |

### Hinweise

Wenn die Breite oder Höhe null ist oder das Diagramm laut Supported Charts List nicht unterstützt wird, führt diese Methode nichts aus. HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode ToImage(string,ImageOrPrintOptions) mit der angegebenen Qualität. Diese Methode wird 12 Monate später, seit März 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodToImageWithStringInt64Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // Rufen Sie die Methode ToImage mit den Parametern (String, Int64) auf.
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Erstellt das Diagrammbild und speichert es in einen Stream im Jpeg-Format.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Ausgabestream. |
| jpegQuality | Int64 | Jpeg-Qualität. |

### Hinweise

Wenn Breite oder Höhe null ist oder das Diagramm laut unterstützter Diagrammliste nicht unterstützt wird, führt diese Methode nichts aus.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamInt64Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Einen Memory-Stream erstellen, um das Bild zu speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    // Rufen Sie die Methode ToImage mit Stream- und Int64-Parametern auf.
                    // Die JPEG-Qualität ist mit 80 angegeben (gültiger Bereich ist typischerweise 0‑100).
                    chart.ToImage(stream, 80);

                    // Erfolgsmeldung anzeigen
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Speichere die Arbeitsmappe
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Ausgabestream. |
| imageFormat | ImageFormat | Das Format, in dem das Bild gespeichert werden soll. |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Chart.ToImage(Stream, ImageType). Diese Eigenschaft wird 12 Monate später, seit Juli 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Einen Memory-Stream erstellen, um das Bild zu speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    // Rufen Sie die Methode ToImage mit Stream- und ImageFormat-Parametern auf.
                    // Verwendung von Aspose.Cells.Drawing.ImageType anstelle von System.Drawing.Imaging.ImageFormat.
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // Erfolgsmeldung anzeigen
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Optional können Sie den Stream zur Überprüfung in einer Datei speichern.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
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

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Ausgabestream. |
| imageType | ImageType | Der Bildtyp, in dem das Bild gespeichert werden soll. |

### Hinweise

Der Bildtyp wird über `imageType` festgelegt. Die folgenden Typen werden unterstützt: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Wenn Breite oder Höhe null ist oder das Diagramm laut unterstützter Diagrammliste nicht unterstützt wird, führt diese Methode nichts aus.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Einen Memory-Stream erstellen, um das Bild zu speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    // Rufen Sie die Methode ToImage mit Stream- und ImageType-Parametern auf.
                    chart.ToImage(stream, ImageType.Png);

                    // Erfolgsmeldung anzeigen
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // Speichern Sie das Bild in einer Datei zur Demonstration.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // Speichere die Arbeitsmappe
                workbook.Save("ChartToImageDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Bildformat.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| imageFile | String | Der Bilddateiname mit vollständigem Pfad. |
| Optionen | ImageOrPrintOptions | Zusätzliche Optionen zur Bildgenerierung |

### Hinweise

Das Format des Bildes wird anhand der Dateierweiterung festgelegt. Beispiel: Wenn Sie "myfile.png" angeben, wird das Bild im PNG‑Format gespeichert. Die folgenden Dateierweiterungen werden erkannt: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Wenn die Breite oder Höhe null ist oder das Diagramm laut Supported Charts List nicht unterstützt wird, führt diese Methode nichts aus. Bitte beachten Sie die [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Bildoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // Laden Sie die Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen und ein Diagramm erstellen
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

            // Diagramm als Bild speichern.
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Der Ausgabestream. |
| Optionen | ImageOrPrintOptions | Zusätzliche Optionen zur Bildgenerierung |

### Hinweise

Der Bildtyp wird durch die Verwendung von `options.ImageType` angegeben. Die folgenden Formate werden unterstützt: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Wenn die Breite oder Höhe null ist oder das Diagramm laut Supported Charts List nicht unterstützt wird, führt diese Methode nichts aus. Bitte beachten Sie die [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) für weitere Details.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageOrPrintOptDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Einen Memory-Stream erstellen, um das Bild zu speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    // Erstellen Sie ImageOrPrintOptions mit spezifischen Einstellungen.
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // Rufen Sie die Methode ToImage mit Stream- und ImageOrPrintOptions-Parametern auf.
                    chart.ToImage(stream, options);

                    // Erfolgsmeldung anzeigen
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Speichere die Arbeitsmappe
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


