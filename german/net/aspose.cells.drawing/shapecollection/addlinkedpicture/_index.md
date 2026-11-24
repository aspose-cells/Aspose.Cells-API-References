---
title: "ShapeCollection.AddLinkedPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein verknüpftes Bild hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Füge ein verknüpftes Bild hinzu.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| Höhe | Int32 | Die Höhe des Shapes. In Pixeln |
| Breite | Int32 | Die Breite des Shapes. In Pixeln |
| sourceFullName | String | Der Pfad und Name der Quelldatei für das verknüpfte Bild |

### Rückgabewert

[`Picture`](../../picture/) Picture object.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext in Zelle A1 hinzufügen
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Verknüpftes Bild zum Arbeitsblatt hinzufügen
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### Siehe auch

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


