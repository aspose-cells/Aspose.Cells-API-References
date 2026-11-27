---
title: "EquationNode.GetChild"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode-metod. Returnerar noden på det angivna indexet bland barnen till den aktuella noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/getchild/
---
## EquationNode.GetChild method

Returnerar noden på det angivna indexet bland den aktuella nodens barn.

```csharp
public EquationNode GetChild(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Index för noden |

### Returvärde

Returnerar motsvarande nod om den angivna noden finns, annars returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodGetChildWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Hämta ekvationsstycket och dess första barnnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Lägg till en avgränsningsnod som barn
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            
            // Lägg till en bråknod inuti avgränsaren
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            FractionEquationNode fractionNode = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);
            
            // Lägg till täljare och nämnare
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textNode = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textNode.Text = "X";
            
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            textNode = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textNode.Text = "Y";
            
            // Spara arbetsboken
            workbook.Save("EquationNodeGetChildDemo.xlsx");
            
            // Läs in den sparade filen för att verifiera
            Workbook loadedWorkbook = new Workbook("EquationNodeGetChildDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Demonstrera GetChild-metoden
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            DelimiterEquationNode loadedDelimiter = (DelimiterEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Delimiter BeginChar: " + loadedDelimiter.BeginChar);
            Console.WriteLine("Delimiter EndChar: " + loadedDelimiter.EndChar);
            
            EquationNode loadedBaseNode = loadedDelimiter.GetChild(0);
            FractionEquationNode loadedFraction = (FractionEquationNode)loadedBaseNode.GetChild(0);
            
            Console.WriteLine("Fraction node type: " + loadedFraction.EquationType);
        }
    }
}
```

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


