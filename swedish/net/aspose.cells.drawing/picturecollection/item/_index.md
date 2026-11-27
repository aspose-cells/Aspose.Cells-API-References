---
title: "PictureCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PictureCollection egenskap. Hämtar Picture-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Hämtar [`Picture`](../../picture/) elementet på det angivna indexet.

```csharp
public Picture this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta bildsamling
            PictureCollection pictures = worksheet.Pictures;
            
            // Lägg till en bild (ersätt "image.png" med den faktiska bildsökvägen)
            int index = pictures.Add(1, 1, "image.png");
            
            // Åtkomst till bilden med Item-egenskapen
            Picture pic = pictures[index];
            
            // Demonstrera användning av Item-egenskapen
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // Ändra bildens egenskaper
            pic.Height = 200;
            pic.Width = 300;
            
            // Spara arbetsboken
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


