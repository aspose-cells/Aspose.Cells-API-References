---
title: "BarEquationNode.BarPosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BarEquationNode-egenskap. Detta attribut anger positionen för stapeln i stapelobjektet"
type: docs
url: /sv/net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

Detta attribut specificerar positionen för stapeln i stapelobjektet

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsnoden
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Skapa en bar ekvationsnod
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            
            // Ställ in stapelns position till Top
            barNode.BarPosition = EquationCharacterPositionType.Top;

            // Lägg till basinnehåll för stapeln
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Spara arbetsboken
            workbook.Save("BarEquationDemo.xlsx");

            // Verifiera den sparade filen
            Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
            Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Se även

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


