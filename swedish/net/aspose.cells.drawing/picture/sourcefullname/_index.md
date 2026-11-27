---
title: "Picture.SourceFullName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskap. Hämtar eller anger sökvägen och namnet på källfilen för den länkade bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Hämtar eller anger sökväg och namn för källfilen till den länkade bilden.

```csharp
public string SourceFullName { get; set; }
```

### Anmärkningar

Standardvärdet är en tom sträng. Om SourceFullName inte är en tom sträng, länkas bilden. Om SourceFullName inte är en tom sträng, men Data är null, länkas bilden och lagras inte i filen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en länkad bild i arbetsbladet
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // Demonstrera SourceFullName-egenskapen
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


