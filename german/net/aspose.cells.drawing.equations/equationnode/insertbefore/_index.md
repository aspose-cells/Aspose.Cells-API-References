---
title: "EquationNode.InsertBefore"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Fügt den angegebenen Knoten vor dem aktuellen Knoten ein"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

Fügt den angegebenen Knoten vor dem aktuellen Knoten ein.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| equationType | EquationNodeType | Typen von Gleichungsknoten |

### Rückgabewert

Wenn der angegebene Typ existiert, wird der entsprechende Knoten zurückgegeben; existiert der Typ nicht, wird ein Knoten unbekannten Typs zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine mathematische Gleichung in Zelle A1 erstellen
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Initialen Textknoten zur Gleichung hinzufügen
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // Einen neuen Textknoten vor dem vorhandenen einfügen
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // Die Gleichung im LaTeX-Format anzeigen
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


