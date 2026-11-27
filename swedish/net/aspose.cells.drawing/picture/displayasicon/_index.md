---
title: "Picture.DisplayAsIcon"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Sant om det angivna objektet visas som en ikon och bilden inte kommer att ändras automatiskt"
type: docs
url: /sv/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

Sant om det angivna objektet visas som en ikon och bilden inte kommer att ändras automatiskt.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Ställ in DisplayAsIcon-egenskapen till sant
            picture.DisplayAsIcon = true;
            
            // Ställ in andra Picture-egenskaper
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // Spara arbetsboken
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


