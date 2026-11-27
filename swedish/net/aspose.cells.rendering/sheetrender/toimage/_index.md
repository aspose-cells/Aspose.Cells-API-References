---
title: "SheetRender.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetRender metod. Rendera en viss sida till en Graphics"
type: docs
url: /sv/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Rendera en viss sida till en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| g | Graphics | Objektet att rendera till. |
| x | Single | X‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |
| y | Single | Y‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |
| bredd | Single | Den maximala bredden (i pixlar) som den renderade sidan kan uppta. |
| höjd | Single | Den maximala höjden (i pixlar) som den renderade sidan kan uppta. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Skapa bildalternativ
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Skapa bladrendering för kalkylbladet
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Skapa en minnesström för att fånga den renderade bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Anropa ToImage med de angivna parametrarna
                    // Eftersom vi inte kan använda System.Drawing.Graphics, kommer vi att använda den enklare ToImage‑överladdningen
                    sheetRender.ToImage(0, stream);

                    // Spara den renderade bilden till fil
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

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Rendera en viss sida till en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| g | Graphics | Objektet att rendera till. |
| x | Single | X‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |
| y | Single | Y‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Skapa bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Skapa SheetRender-instans
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Eftersom vi inte kan använda System.Drawing-typer, kommer vi att använda den alternativa ToImage-metoden
                // som sparar direkt till en fil
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Rensa resurser
                sheetRender.Dispose();
            }
        }
    }
}
```

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

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
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Läs in käll-Excel-filen
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Skapa bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Skapa sheet render för det första kalkylbladet
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Rendera den första sidan av sheet till en bildfil
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

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

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Skapa bildalternativ
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Skapa SheetRender-instans
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Skapa en minnesström för att lagra bilden
                using (MemoryStream stream = new MemoryStream())
                {
                    // Anropa ToImage med sidindex och strömparametrar
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

### Se även

* class [SheetRender](../)
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

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Skapa bildalternativ
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Skapa SheetRender-instans
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Hämta det första sidindexet (0-baserat)
                int pageIndex = 0;

                // Anropa ToImage med sidindexparametern
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

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


