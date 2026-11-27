---
title: "Enum EquationHorizontalJustificationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationHorizontalJustificationType enum. Detta anger standardhorisontell justering av ekvationer i dokumentet"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationhorizontaljustificationtype/
---
## EquationHorizontalJustificationType enumeration

Detta specificerar standardhorisontell justering av ekvationer i dokumentet.

```csharp
public enum EquationHorizontalJustificationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Center | `0` | Centrerad |
| CenterGroup | `1` | Centrerad som grupp |
| Left | `2` | Vänsterjusterad |
| Right | `3` | Högerjusterad |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationHorizontalJustificationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en ekvationsform till kalkylbladet
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Hämta ekvationsstycket
                EquationNodeParagraph equationNode = (EquationNodeParagraph)textBox.GetEquationParagraph();

                // Demonstrera olika horisontella justeringstyper
                equationNode.Justification = EquationHorizontalJustificationType.Center;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Left;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Right;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                // Spara arbetsboken
                workbook.Save("EquationHorizontalJustificationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationHorizontalJustificationType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


