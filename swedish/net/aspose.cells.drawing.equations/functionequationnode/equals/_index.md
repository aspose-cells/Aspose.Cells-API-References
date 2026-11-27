---
title: "FunctionEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FunctionEquationNode-metod. Avgör om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/functionequationnode/equals/
---
## FunctionEquationNode.Equals method

Bestäm om den aktuella ekvationsnoden är lika med den angivna noden

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | Den angivna noden |

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox-form för att innehålla en ekvation
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 200, 100);

            // Hämta rot‑ekvationsnoden för TextBoxen
            EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa den första funktions‑ekvationsnoden
            FunctionEquationNode funcNode1 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            // (Valfritt) Lägg till minimalt innehåll för att göra noden giltig
            EquationNode funcName1 = funcNode1.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText1 = (TextRunEquationNode)funcName1.AddChild(EquationNodeType.Text);
            nameText1.Text = "Sin";

            // Skapa den andra funktions‑ekvationsnoden
            FunctionEquationNode funcNode2 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            EquationNode funcName2 = funcNode2.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText2 = (TextRunEquationNode)funcName2.AddChild(EquationNodeType.Text);
            nameText2.Text = "Cos";

            try
            {
                // Jämför de två funktionsnoderna med Equals(Object)
                bool areEqual = funcNode1.Equals((object)funcNode2);
                Console.WriteLine($"funcNode1.Equals(funcNode2) returned: {areEqual}");

                // Jämför en nod med sig själv
                bool selfEqual = funcNode1.Equals((object)funcNode1);
                Console.WriteLine($"funcNode1.Equals(funcNode1) returned: {selfEqual}");

                // Spara arbetsboken (inga visuella ändringar behövs för denna demo)
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

### Se även

* class [FunctionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


