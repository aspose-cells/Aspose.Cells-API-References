---
title: "ShapeCollection.AddFreeform"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt dem Arbeitsblatt eine Freiformform hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Fügt eine Freiformform zum Arbeitsblatt hinzu.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz der Freiformform von ihrer linken Zeile in Pixeln dar. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz der Freiformform von ihrer linken Spalte in Pixeln dar. |
| Höhe | Int32 | Stellt die Höhe der Freiformform in Pixeln dar. |
| Breite | Int32 | Stellt die Breite der Freiformform in Pixeln dar. |
| Pfade | ShapePath[] | Stellt einen benutzerdefinierten Pfad dar |

### Rückgabewert

Eine Freiformform.

### Hinweise

Hinweis: Die Breite und Höhe in den Parametern können beliebige positive Ganzzahlen sein, nicht die gesamte Breite und Höhe des durch ’paths' angegebenen ShapePath‑Arrays. Die Beziehung zwischen ihnen ist eine Skalierungs‑Füll‑Beziehung, d.h., jedes ShapePath‑Objekt wird entsprechend der Breite und Höhe skaliert. Daher muss, wenn mehrere Objekte im 'paths' vorhanden sind, jedes ShapePath‑Objekt vernünftig gestaltet werden, um den Erwartungen zu entsprechen. Ist nur ein ShapePath‑Objekt vorhanden und gibt es keine weiteren Anforderungen, ist das Übergeben der Breite und Höhe des Objekts als Parameterwerte eine gute Lösung.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Benutzerdefinierte Figurenpfade erstellen
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // Freiformform zum Arbeitsblatt hinzufügen
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // Speichere die Arbeitsmappe
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


