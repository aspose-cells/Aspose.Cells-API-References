---
title: "Picture.IsAutoSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Sant indikerar att storleken på ole-objektet automatiskt ändras i takt med storleken på ögonblicksbilden av det inbäddade innehållet när ole-objektet aktiveras"
type: docs
url: /sv/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

Sant indikerar att storleken på OLE-objektet automatiskt ändras till storleken på en ögonblicksbild av det inbäddade innehållet när OLE-objektet aktiveras.

```csharp
public bool IsAutoSize { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Demonstrera IsAutoSize-egenskap
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // Ställ in IsAutoSize till true - bilden kommer automatiskt att ändra storlek för att passa sitt innehåll
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // Ställ in IsAutoSize till false - bilden behåller sina ursprungliga dimensioner
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // Spara arbetsboken
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


