---
title: "ShapeCollection.AddOleObjectWithLinkedImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection‑metod. Lägg till en länkad bild"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage/
---
## ShapeCollection.AddOleObjectWithLinkedImage method

Lägg till en länkad bild.

```csharp
public OleObject AddOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, 
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddOleObjectWithLinkedImageWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sökväg till bildfilen som ska länkas
            string imagePath = "example.jpg";

            try
            {
                // Anropa metoden AddOleObjectWithLinkedImage med specifika parametrar
                OleObject oleObject = worksheet.Shapes.AddOleObjectWithLinkedImage(
                    1,  // upperLeftRow
                    1,  // upperLeftColumn
                    200, // height
                    300, // width
                    imagePath); // sourceFullName

                // Ange ytterligare egenskaper för OleObject
                oleObject.DisplayAsIcon = false;
                oleObject.IsAutoSize = true;

                Console.WriteLine("OLE object with linked image added successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddOleObjectWithLinkedImage method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("AddOleObjectWithLinkedImageDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


