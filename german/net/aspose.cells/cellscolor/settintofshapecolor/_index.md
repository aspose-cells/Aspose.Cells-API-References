---
title: "CellsColor.SetTintOfShapeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsColor-Methode. Setzt den Farbton der Formfarbe"
type: docs
url: /de/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

Setzen Sie den Farbton der Formfarbe

```csharp
public void SetTintOfShapeColor(double tint)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbton | Double |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Holen Sie die Füllfarbe der Form
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // Setzen Sie die Farbe, die als Formfarbe behandelt wird
                shapeColor.IsShapeColor = true;
                
                // Setzen Sie den Farbton der Formfarbe (gültiger Bereich ist -1,0 bis 1,0)
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // Zeigen Sie den Effekt, indem Sie die Füllfarbe der Form ändern
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


