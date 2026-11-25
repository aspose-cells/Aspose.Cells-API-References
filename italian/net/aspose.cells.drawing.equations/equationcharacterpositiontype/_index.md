---
title: "Enum EquationCharacterPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Equations.EquationCharacterPositionType enum. Specifica la posizione di un particolare sottooggetto all'interno del suo genitore"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationcharacterpositiontype/
---
## EquationCharacterPositionType enumeration

Specifica la posizione di un particolare sottooggetto all'interno del suo genitore

```csharp
public enum EquationCharacterPositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Top | `0` | Nella parte superiore dell'oggetto genitore |
| Bottom | `1` | Nella parte inferiore dell'oggetto genitore |

### Esempi

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
            
            // Aggiungi forma dell'equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Ottieni il nodo dell'equazione e aggiungi una barra con posizione superiore
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            barNode.BarPosition = EquationCharacterPositionType.Top;
            
            // Aggiungi testo di base
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";
            
            // Salva e verifica
            string outputFile = "EquationCharacterPositionTypeDemo.xlsx";
            workbook.Save(outputFile);
            
            // Ricarica e verifica
            Workbook loadedWorkbook = new Workbook(outputFile);
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode loadedBarNode = (BarEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + loadedBarNode.BarPosition);
            Console.WriteLine("Text Content: " + ((TextRunEquationNode)loadedBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


