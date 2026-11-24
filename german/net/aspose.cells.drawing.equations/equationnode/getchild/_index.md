---
title: "EquationNode.GetChild"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNode-Methode. Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnode/getchild/
---
## EquationNode.GetChild method

Gibt den Knoten am angegebenen Index unter den Kindknoten des aktuellen Knotens zurück.

```csharp
public EquationNode GetChild(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Index des Knotens |

### Rückgabewert

Gibt den entsprechenden Knoten zurück, wenn der angegebene Knoten existiert, andernfalls wird null zurückgegeben.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie dem ersten Arbeitsblatt eine Gleichungsform hinzu.
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Hole den Gleichungsabsatz und seinen ersten Kindknoten
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Füge einen Trennzeichenknoten als Kind hinzu
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            
            // Füge einen Bruchknoten innerhalb des Trennzeichens hinzu
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            FractionEquationNode fractionNode = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);
            
            // Füge Zähler und Nenner hinzu
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textNode = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textNode.Text = "X";
            
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            textNode = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textNode.Text = "Y";
            
            // Speichere die Arbeitsmappe
            workbook.Save("EquationNodeGetChildDemo.xlsx");
            
            // Lade die gespeicherte Datei zum Überprüfen
            Workbook loadedWorkbook = new Workbook("EquationNodeGetChildDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Demonstriere die GetChild-Methode
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

### Siehe auch

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


