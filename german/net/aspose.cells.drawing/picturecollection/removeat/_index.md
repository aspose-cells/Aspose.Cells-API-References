---
title: "PictureCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PictureCollection method. Entfernt Formen am angegebenen Index"
type: docs
url: /de/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

Entferne Formen am angegebenen Index

```csharp
public void RemoveAt(int index)
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Bilder zum Arbeitsblatt hinzu
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // Entferne das Bild am angegebenen Index
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


