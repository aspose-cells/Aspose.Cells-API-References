---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Optimera html-utdata genom att använda CSS-anpassade egenskaper. Till exempel, i scenariot där det finns flera förekomster av en base64-bild med en anpassad egenskap, behöver bilddata bara sparas en gång, så prestandan för den resulterande html kan förbättras. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

Optimera html‑utdata genom att använda CSS‑anpassade egenskaper. Till exempel, i scenariot där en base64‑bild förekommer flera gånger, krävs bilddata endast sparas en gång med en anpassad egenskap, vilket kan förbättra prestandan för den resulterande html‑filen. Standardvärdet är false.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med formatering
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // Lägg till en bild som kommer att upprepas i flera celler
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // Kopiera bilden till en annan plats
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // Skapa en HtmlSaveOptions-instans
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // Visa aktuellt värde
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // Ställ in till true för att optimera CSS-utdata
            htmlOptions.EnableCssCustomProperties = true;

            // Spara med CSS-optimering
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // Ställ in till false för jämförelse
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


