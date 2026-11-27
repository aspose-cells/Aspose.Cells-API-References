---
title: "FontFileDataInfo.Data"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontFileDataInfo-egenskapen. Hämtar binär data för teckensnittsfilen"
type: docs
url: /sv/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

Hämtar binärdata för teckensnittsfilen.

```csharp
public byte[] Data { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Läs in en teckensnittsfil (ersätt med den faktiska sökvägen till teckensnittsfilen)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Skapa en FontConfigs-instans och lägg till teckensnittet
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // I verklig användning skulle FontFileDataInfo hämtas från biblioteket
            // För demonstrationsändamål visar vi bara hur du skulle använda den om du hade en
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // Visa information om teckensnittsdata (om tillgänglig)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // I verklig användning skulle Data-egenskapen användas för att komma åt teckensnittets binära data
            // Till exempel kan du spara den till en fil:
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // Spara arbetsboken (teckensnittet skulle påverka rendering om det används i celler)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


