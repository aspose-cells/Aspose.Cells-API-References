---
title: "BarEquationNode.BarPosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BarEquationNode-Eigenschaft. Dieses Attribut gibt die Position des Balkens im Balkenobjekt an"
type: docs
url: /de/net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

Dieses Attribut gibt die Position des Balkens im Balkenobjekt an

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class BarEquationNodePropertyBarPositionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie dem ersten Arbeitsblatt eine Gleichungsform hinzu.
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Den Gleichungsknoten abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Erstelle einen Bar-Gleichungsknoten
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            
            // Setze die Bar-Position auf Top
            barNode.BarPosition = EquationCharacterPositionType.Top;

            // Füge Basisinhalt für die Leiste hinzu
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Speichere die Arbeitsmappe
            workbook.Save("BarEquationDemo.xlsx");

            // Überprüfen Sie die gespeicherte Datei
            Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
            Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Siehe auch

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


