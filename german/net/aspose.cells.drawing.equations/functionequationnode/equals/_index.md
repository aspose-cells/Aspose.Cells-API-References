---
title: "FunctionEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FunctionEquationNode-Methode. Bestimmen Sie, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/functionequationnode/equals/
---
## FunctionEquationNode.Equals method

Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Der angegebene Knoten |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FunctionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein TextBox-Shape hinzu, um eine Gleichung zu halten
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 200, 100);

            // Ermitteln Sie den Wurzel-Gleichungsknoten der TextBox
            EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

            // Erstellen Sie den ersten Funktionsgleichungsknoten
            FunctionEquationNode funcNode1 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            // (Optional) Fügen Sie minimalen Inhalt hinzu, um den Knoten gültig zu machen
            EquationNode funcName1 = funcNode1.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText1 = (TextRunEquationNode)funcName1.AddChild(EquationNodeType.Text);
            nameText1.Text = "Sin";

            // Erstellen Sie den zweiten Funktionsgleichungsknoten
            FunctionEquationNode funcNode2 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            EquationNode funcName2 = funcNode2.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText2 = (TextRunEquationNode)funcName2.AddChild(EquationNodeType.Text);
            nameText2.Text = "Cos";

            try
            {
                // Vergleichen Sie die beiden Funktionsknoten mit Equals(Object)
                bool areEqual = funcNode1.Equals((object)funcNode2);
                Console.WriteLine($"funcNode1.Equals(funcNode2) returned: {areEqual}");

                // Vergleichen Sie einen Knoten mit sich selbst
                bool selfEqual = funcNode1.Equals((object)funcNode1);
                Console.WriteLine($"funcNode1.Equals(funcNode1) returned: {selfEqual}");

                // Speichern Sie die Arbeitsmappe (keine visuellen Änderungen für diese Demo erforderlich)
                workbook.Save("FunctionEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [FunctionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


