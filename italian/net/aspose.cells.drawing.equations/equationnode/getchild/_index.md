---
title: "EquationNode.GetChild"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Restituisce il nodo all'indice specificato tra i figli del nodo corrente"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/getchild/
---
## EquationNode.GetChild method

Restituisce il nodo all'indice specificato tra i figli del nodo corrente.

```csharp
public EquationNode GetChild(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | Indice del nodo |

### Valore di ritorno

Restituisce il nodo corrispondente se il nodo specificato esiste, altrimenti restituisce null.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma di equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Ottieni il paragrafo dell'equazione e il suo primo nodo figlio
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Aggiungi un nodo delimitatore come figlio
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            
            // Aggiungi un nodo frazione all'interno del delimitatore
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            FractionEquationNode fractionNode = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);
            
            // Aggiungi numeratore e denominatore
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textNode = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textNode.Text = "X";
            
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            textNode = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textNode.Text = "Y";
            
            // Salva la cartella di lavoro
            workbook.Save("EquationNodeGetChildDemo.xlsx");
            
            // Carica il file salvato per verificare
            Workbook loadedWorkbook = new Workbook("EquationNodeGetChildDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Dimostra il metodo GetChild
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

### Vedi anche

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


