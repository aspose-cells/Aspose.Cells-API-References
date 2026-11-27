---
title: "Enum EquationVerticalJustificationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationVerticalJustificationType-enum. Detta specificerar standardvertikaljustering av ekvationer i dokumentet."
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationverticaljustificationtype/
---
## EquationVerticalJustificationType enumeration

Detta specificerar standardvertikal justering av ekvationer i dokumentet.

```csharp
public enum EquationVerticalJustificationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Top | `0` | top |
| Center | `1` | center |
| Bottom | `2` | bottom |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationVerticalJustificationTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationstycket och lägg till en matrisnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Ställ in matrisens egenskaper
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Lägg till matrisrader och kolumner.
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // Spara arbetsboken
            string outputPath = "EquationVerticalJustificationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("File saved with vertical justification demo: " + outputPath);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


