---
title: "OleObjectCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObjectCollection-metod. Tar bort elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.drawing/oleobjectcollection/removeat/
---
## OleObjectCollection.RemoveAt method

Tar bort elementet på det angivna indexet.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Det angivna indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempel OLE-objekt (3 objekt)
            for (int i = 0; i < 3; i++)
            {
                sheet.OleObjects.Add(i * 10, i * 10, 100, 100, new byte[0]);
            }

            Console.WriteLine("Before removal - OLE Objects count: " + sheet.OleObjects.Count);
            
            // Ta bort OLE-objekt ett i taget med RemoveAt(int index)
            for (int i = sheet.OleObjects.Count - 1; i >= 0; i--)
            {
                sheet.OleObjects.RemoveAt(i);
            }

            Console.WriteLine("After removal - OLE Objects count: " + sheet.OleObjects.Count);
        }
    }
}
```

### Se även

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


