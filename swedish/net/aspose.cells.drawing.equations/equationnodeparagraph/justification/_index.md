---
title: "EquationNodeParagraph.Justification"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNodeParagraph egenskap. Detta specificerar justeringen av matematik‑paragrafen, en serie av intilliggande ekvationer inom samma paragraf. En matematik‑paragraf kan vara Left Justified, Right Justified, Centered eller Centered as Group. Som standard är matematik‑paragrafen Centered as Group. Detta innebär att ekvationerna kan justeras i förhållande till varandra men hela gruppen av ekvationer är centrerad som helhet"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

Detta specificerar justeringen av det matematiska stycket (en serie av intilliggande ekvationer inom samma stycke). Ett matematiskt stycke kan vara vänsterjusterat, högerjusterat, centrerat eller centrerat som grupp. Som standard är det matematiska stycket centrerat som grupp. Detta innebär att ekvationerna kan justeras i förhållande till varandra, men hela gruppen av ekvationer är centrerad som helhet.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hålla ekvationen
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Hämta ekvationsstycket
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // Visa aktuellt justeringsvärde
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // Ställ in olika justeringsvärden och observera effekterna
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // Spara arbetsboken
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### Se även

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


