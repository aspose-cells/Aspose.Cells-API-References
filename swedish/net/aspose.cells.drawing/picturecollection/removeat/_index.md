---
title: "PictureCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PictureCollection metod. Tar bort former på ett specifikt index"
type: docs
url: /sv/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

Ta bort former vid det specifika indexet

```csharp
public void RemoveAt(int index)
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några bilder i arbetsbladet
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // Ta bort bilden på angivet index
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


