---
title: "ShapePath.PathSegementList"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath-Eigenschaft. Gibt ShapeSegmentPathCollection-Liste zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

Gibt die [`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/) Liste zurück

```csharp
[Obsolete("Use ShapePath.PathSegments property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ShapeSegmentPathCollection PathSegementList { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die ShapePath.PathSegments‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Erstellen Sie einen neuen Formpfad
                ShapePath shapePath = new ShapePath();

                // Zum Ausgangspunkt bewegen
                shapePath.MoveTo(10, 10);

                // Rufen Sie die LineTo-Methode mit (Single, Single)-Parametern auf
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // Greifen Sie auf die PathSegementList-Eigenschaft zu
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // Anzahl der Pfadsegmente anzeigen
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // Durchlaufen Sie jedes Segment und zeigen Sie dessen Typ an
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //Freiform hinzufügen
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


