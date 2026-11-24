---
title: "OleObjectCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObjectCollection-Methode. Entfernt das Element am angegebenen Index"
type: docs
url: /de/net/aspose.cells.drawing/oleobjectcollection/removeat/
---
## OleObjectCollection.RemoveAt method

Entfernt das Element am angegebenen Index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der angegebene Index. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispiel-OLE-Objekte hinzufügen (3 Objekte)
            for (int i = 0; i < 3; i++)
            {
                sheet.OleObjects.Add(i * 10, i * 10, 100, 100, new byte[0]);
            }

            Console.WriteLine("Before removal - OLE Objects count: " + sheet.OleObjects.Count);
            
            // Entfernen Sie OLE-Objekte nacheinander mit RemoveAt(int index)
            for (int i = sheet.OleObjects.Count - 1; i >= 0; i--)
            {
                sheet.OleObjects.RemoveAt(i);
            }

            Console.WriteLine("After removal - OLE Objects count: " + sheet.OleObjects.Count);
        }
    }
}
```

### Siehe auch

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


