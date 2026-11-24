---
title: "EquationNode.CreateNode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Erstellt einen Knoten des angegebenen Typs"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

Erstellen Sie einen Knoten des angegebenen Typs.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| equationType | EquationNodeType | Typen von Gleichungsknoten |
| Arbeitsmappe | Arbeitsmappe | Das Arbeitsmappenobjekt, das mit der Gleichung verknüpft ist |
| Eltern | EquationNode | Der übergeordnete Knoten, in dem sich dieser Knoten befindet |

### Rückgabewert

Wenn der angegebene Typ existiert, wird der entsprechende Knoten zurückgegeben; existiert der Typ nicht, wird ein Knoten unbekannten Typs zurückgegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Gleichungsform erstellen
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Einen Elternknoten (Bruch) erstellen
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // Erstelle Zähler- und Nennerknoten
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // Füge den erstellten Bruch zur Hauptgleichung hinzu
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // Gleichung in einer Zelle anzeigen
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


