---
title: "ShapeCollection.AddOleObjectWithLinkedImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt ein verknüpftes Bild hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage/
---
## ShapeCollection.AddOleObjectWithLinkedImage method

Füge ein verknüpftes Bild hinzu.

```csharp
public OleObject AddOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, 
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddOleObjectWithLinkedImageWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pfad zur Bilddatei, die verlinkt werden soll
            string imagePath = "example.jpg";

            try
            {
                // Rufen Sie die Methode AddOleObjectWithLinkedImage mit spezifischen Parametern auf
                OleObject oleObject = worksheet.Shapes.AddOleObjectWithLinkedImage(
                    1,  // upperLeftRow
                    1,  // upperLeftColumn
                    200, // height
                    300, // width
                    imagePath); // sourceFullName

                // Setzen Sie zusätzliche Eigenschaften für das OleObject
                oleObject.DisplayAsIcon = false;
                oleObject.IsAutoSize = true;

                Console.WriteLine("OLE object with linked image added successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddOleObjectWithLinkedImage method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("AddOleObjectWithLinkedImageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


