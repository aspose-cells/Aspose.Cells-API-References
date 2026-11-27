---
title: "Chart.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagrammetod. Hämtar ett 32‑bit Bitmap‑objekt av diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Hämtar ett 32‑bit `Bitmap`‑objekt av diagrammet.

```csharp
public Bitmap ToImage()
```

### Returvärde

bilden av diagrammet.

### Anmärkningar

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den att returnera null.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:B4", true);
            
            // Konvertera diagram till bild och spara till fil
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Hämtar ett 32‑bit `Bitmap`‑objekt av diagrammet. `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression och ImageOrPrintOptions.Quality‑attribut ignoreras.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | ImageOrPrintOptions | Ytterligare alternativ för bildskapande |

### Returvärde

bilden av diagrammet.

### Anmärkningar

Returnerar ett 32‑bit bitmap‑objekt, så påverkas inte metoden av attributen ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression och ImageOrPrintOptions.Quality. Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den att returnera null.

### Exempel

Hämtar ett bitmap‑objekt med 200 x dpi och 300 y dpi.

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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Skapar diagrammets bild och sparar den till en fil. Filnamnets filändelse bestämmer bildens format.

```csharp
public void ToImage(string imageFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |

### Anmärkningar

Bildens format anges genom att använda filnamnets filändelse. Till exempel, om du anger \"myfile.png\", sparas bilden i PNG‑formatet. Följande filändelser känns igen: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra någonting.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Spara diagram som bild
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

Skapar diagrammets bild och sparar den till en fil i angivet format.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |
| imageFormat | ImageFormat | Formatet att spara bilden i. |

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället metoden Chart.ToImage(string, ImageType). Denna egenskap kommer att tas bort 12 månader senare från och med juli 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Skapar diagrammets bild och sparar den till en fil i den angivna bildtypen.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |
| imageType | ImageType | Bildtypen att spara bilden i. |

### Anmärkningar

Bildens typ anges genom att använda `imageType`. Följande typer stöds: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra någonting.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Spara diagram till bild med angiven ImageType
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### Se även

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Skapar diagrammets bild och sparar den till en fil i Jpeg-format.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |
| jpegQuality | Int64 | Jpeg-kvalitet. |

### Anmärkningar

Om bredden eller höjden är noll eller diagrammet inte stöds enligt Supported Charts List, kommer denna metod inte göra någonting. OBS: Denna metod är nu föråldrad. Använd i stället ToImage(string,ImageOrPrintOptions)-metoden med angiven kvalitet. Denna metod kommer att tas bort 12 månader senare från och med mars 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // Anropa ToImage-metoden med parametrarna (String, Int64)
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Skapar diagrammets bild och sparar den till en ström i Jpeg-format.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen. |
| jpegQuality | Int64 | Jpeg-kvalitet. |

### Anmärkningar

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra någonting.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Skapa en minnesström för att spara bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Anropa ToImage-metoden med Stream- och Int64-parametrar.
                    // JPEG-kvaliteten anges som 80 (giltigt intervall är vanligtvis 0‑100)
                    chart.ToImage(stream, 80);

                    // Visa framgångsmeddelande
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Spara arbetsboken
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

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

Skapar diagrammets bild och sparar den till en ström i det angivna formatet.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen. |
| imageFormat | ImageFormat | Formatet att spara bilden i. |

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället Chart.ToImage(Stream, ImageType)-metoden. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Skapa en minnesström för att spara bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Anropa ToImage-metoden med Stream- och ImageFormat-parametrar.
                    // Använd Aspose.Cells.Drawing.ImageType istället för System.Drawing.Imaging.ImageFormat.
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // Visa framgångsmeddelande
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Spara eventuellt streamen till en fil för verifiering.
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

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Skapar diagrammets bild och sparar den till en ström i det angivna formatet.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen. |
| imageType | ImageType | Bildtypen att spara bilden i. |

### Anmärkningar

Bildens typ anges genom att använda `imageType`. Följande typer stöds: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer denna metod inte att göra någonting.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Skapa en minnesström för att spara bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Anropa ToImage-metoden med Stream- och ImageType-parametrar.
                    chart.ToImage(stream, ImageType.Png);

                    // Visa framgångsmeddelande
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // Spara bilden till en fil för demonstration.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // Spara arbetsboken
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

### Se även

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Skapar diagrammets bild och sparar den till en fil. Filnamnets filändelse bestämmer bildens format.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | String | Bildfilens namn med fullständig sökväg. |
| alternativ | ImageOrPrintOptions | Ytterligare alternativ för bildskapande |

### Anmärkningar

Bildens format anges genom att använda filnamnets filändelse. Till exempel, om du anger \"myfile.png\", sparas bilden i PNG‑formatet. Följande filändelser känns igen: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Om bredden eller höjden är noll eller diagrammet inte stöds enligt Supported Charts List, kommer denna metod inte göra någonting. Se gärna [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Exempel

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
            // Skapa bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // Läs in arbetsboken
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

            // Spara diagram till bild.
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Skapar diagrammets bild och sparar den till en ström i det angivna formatet.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Utdatastreamen. |
| alternativ | ImageOrPrintOptions | Ytterligare alternativ för bildskapande |

### Anmärkningar

Bildens typ anges genom att använda `options.ImageType`. Följande format stöds: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Om bredden eller höjden är noll eller diagrammet inte stöds enligt Supported Charts List, kommer denna metod inte göra någonting. Se gärna [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer information.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Skapa en minnesström för att spara bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Skapa ImageOrPrintOptions med specifika inställningar.
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // Anropa ToImage-metoden med Stream- och ImageOrPrintOptions-parametrar.
                    chart.ToImage(stream, options);

                    // Visa framgångsmeddelande
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Spara arbetsboken
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

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


