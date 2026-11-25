---
title: "Enum EquationDelimiterShapeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType. Questo specifica la forma dei delimitatori nell'oggetto delimitatore."
type: docs
url: /it/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

Questo specifica la forma dei delimitatori nell'oggetto delimitatore.

```csharp
public enum EquationDelimiterShapeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Centered | `0` | Il divisore è centrato sull'intera altezza del suo contenuto. |
| Match | `1` | Il divisore è modificato per corrispondere esattamente all'altezza dei loro contenuti. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi forma dell'equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Ottieni nodo dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crea nodo delimitatore con tipo di forma Match
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // Aggiungi contenuto all'interno del delimitatore
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // Salva la cartella di lavoro
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


