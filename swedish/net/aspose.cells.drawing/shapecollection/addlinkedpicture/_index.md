---
title: "ShapeCollection.AddLinkedPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection‑metod. Lägg till en länkad bild"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Lägg till en länkad bild.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| höjd | Int32 | Formens höjd. I enhet pixlar |
| bredd | Int32 | Formens bredd. I enhet pixlar |
| sourceFullName | String | Sökvägen och namnet på källfilen för den länkade bilden |

### Returvärde

[`Picture`](../../picture/) Picture object.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeltext i cell A1
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Lägg till länkad bild i kalkylbladet
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Spara arbetsboken
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### Se även

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


