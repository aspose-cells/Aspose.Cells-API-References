---
title: "Enum EquationCharacterPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationCharacterPositionType-enum. Specificerar positionen för ett specifikt delobjekt inom dess förälder"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationcharacterpositiontype/
---
## EquationCharacterPositionType enumeration

Specificerar positionen för ett specifikt delobjekt inom dess förälder

```csharp
public enum EquationCharacterPositionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Top | `0` | Längst upp i föräldraobjektet |
| Bottom | `1` | Längst ner i föräldraobjektet |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationCharacterPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Hämta ekvationsnod och lägg till streck med topposition
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            barNode.BarPosition = EquationCharacterPositionType.Top;
            
            // Lägg till bastext
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";
            
            // Spara och verifiera
            string outputFile = "EquationCharacterPositionTypeDemo.xlsx";
            workbook.Save(outputFile);
            
            // Läs om och verifiera
            Workbook loadedWorkbook = new Workbook(outputFile);
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode loadedBarNode = (BarEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + loadedBarNode.BarPosition);
            Console.WriteLine("Text Content: " + ((TextRunEquationNode)loadedBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


