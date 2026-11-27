---
title: "Picture.IsDynamicDataExchange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskapen. Hämtar eller anger om dynamisk datautbyte"
type: docs
url: /sv/net/aspose.cells.drawing/picture/isdynamicdataexchange/
---
## Picture.IsDynamicDataExchange property

Hämtar eller anger om dynamisk datautbyte

```csharp
public bool IsDynamicDataExchange { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsDynamicDataExchangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Demonstrera IsDynamicDataExchange-egenskapen
            Console.WriteLine("Original IsDynamicDataExchange value: " + picture.IsDynamicDataExchange);
            
            // Ange IsDynamicDataExchange till true
            picture.IsDynamicDataExchange = true;
            Console.WriteLine("After setting IsDynamicDataExchange to true: " + picture.IsDynamicDataExchange);

            // Spara arbetsboken
            workbook.Save("PicturePropertyIsDynamicDataExchangeDemo.xlsx", SaveFormat.Xlsx);

            // Läs in den sparade arbetsboken för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook("PicturePropertyIsDynamicDataExchangeDemo.xlsx");
            Picture loadedPicture = loadedWorkbook.Worksheets[0].Pictures[0];
            Console.WriteLine("Loaded IsDynamicDataExchange value: " + loadedPicture.IsDynamicDataExchange);
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


