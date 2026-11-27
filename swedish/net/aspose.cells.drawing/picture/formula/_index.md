---
title: "Picture.Formula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-egenskapen. Hämtar och anger data för formeln"
type: docs
url: /sv/net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Hämtar och anger data för formeln.

```csharp
public string Formula { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Ange formel för bilden
            picture.Formula = "A1:A3";
            Console.WriteLine("Picture Formula: " + picture.Formula);

            // Ändra formeln
            picture.Formula = "B1:B3";
            Console.WriteLine("Updated Picture Formula: " + picture.Formula);

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


