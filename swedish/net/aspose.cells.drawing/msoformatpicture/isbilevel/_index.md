---
title: "MsoFormatPicture.IsBiLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Anger om bilden ska visas i tvåfärgs svart‑vitt"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Indikerar om den här bilden ska visas i tvåfärgs svartvitt.

```csharp
public bool IsBiLevel { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en bild i arbetsbladet
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Ställ in bilden till tvånivå (svart‑vitt)
            picture.FormatPicture.IsBiLevel = true;
            
            // Verifiera och skriv ut värdet för egenskapen IsBiLevel
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


