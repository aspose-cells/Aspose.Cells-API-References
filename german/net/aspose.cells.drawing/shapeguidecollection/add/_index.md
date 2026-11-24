---
title: "ShapeGuideCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeGuideCollection-Methode. Fügt einen Shape-Guide hinzu. Wichtig: Dieses Feature ist derzeit nur für Excel07 und höher verfügbar"
type: docs
url: /de/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

Fügt einen Shape Guide hinzu. (Wichtig: Diese Funktion ist derzeit nur für Excel07 und höher verfügbar)

```csharp
public int Add(string name, double val)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name von adjust. Er lautet "adj (Verwendet, wenn nur ein Anpassungswert vorhanden ist)", "adj1", "adj2", "adj3" und so weiter. |
| val | Double | Der Wert von adjust |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Form, die Anpassungsführungen verwendet
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // Rufe die ShapeGuideCollection aus den Geometrie-Anpassungen der Form ab
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // Rufe die Add-Methode mit den Parametern (String, Double) auf
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


