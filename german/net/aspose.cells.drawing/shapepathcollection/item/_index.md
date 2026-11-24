---
title: "ShapePathCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathCollection‑Eigenschaft. Gibt einen Erstellungs-Pfad zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Liefert einen Erstellungs-Pfad.

```csharp
public ShapePath this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Gibt das [`ShapePath`](../../shapepath/)‑Objekt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine benutzerdefinierte Form (nicht‑primitive Form) mit korrekten Parametern hinzu
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // Greife auf die ShapePathCollection zu
            ShapePathCollection shapePaths = customShape.Paths;

            // Füge einen neuen Pfad hinzu
            int pathIndex = shapePaths.Add();

            // Greife auf den Pfad über die Item‑Eigenschaft zu
            ShapePath newPath = shapePaths[pathIndex];

            // Ausgabeinformationen
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


