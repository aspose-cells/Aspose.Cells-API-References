---
title: "PageSetup.GetPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Hämtar Picture-objektet för sidhuvudet / sidfoten"
type: docs
url: /sv/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Hämtar [`Picture`](../../../aspose.cells.drawing/picture/) objektet för sidhuvudet / sidfoten.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isHeader | Boolean | Anger om det är i sidhuvudet eller sidfoten. |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |

### Returvärde

Returnerar [`Picture`](../../../aspose.cells.drawing/picture/) objekt. Returnerar null om det inte finns någon bild.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en bild i kalkylbladets sidhuvud
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // Hämta bilden från sidhuvudet och ändra dess ljusstyrka
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Hämtar [`Picture`](../../../aspose.cells.drawing/picture/) objektet för sidhuvudet / sidfoten.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isFirst | Boolean | Anger om bilden för första sidans sidhuvud eller sidfot hämtas. |
| isEven | Boolean | Anger om bilden för jämna sidors sidhuvud eller sidfot hämtas. |
| isHeader | Boolean | Anger om bilden för sidhuvud eller sidfot hämtas. |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |

### Returvärde

Returnerar [`Picture`](../../../aspose.cells.drawing/picture/) objekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta PageSetup-objektet
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in vissa sidhuvuds-/sidfots-egenskaper för att säkerställa att vi har bilder att hämta
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // Anropa GetPicture-metoden med parametrarna: isFirst, isEven, isHeader, section
                // Kontrollerar första sidans sidhuvud (sektion 0 - centrerat sidhuvud)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // Spara arbetsboken
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


