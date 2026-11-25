---
title: "BarEquationNode.BarPosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BarEquationNode. Questo attributo specifica la posizione della barra nell'oggetto barra"
type: docs
url: /it/net/aspose.cells.drawing.equations/barequationnode/barposition/
---
## BarEquationNode.BarPosition property

Questo attributo specifica la posizione della barra nell'oggetto barra

```csharp
public EquationCharacterPositionType BarPosition { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class BarEquationNodePropertyBarPositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma di equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Crea un nodo di equazione barra
            BarEquationNode barNode = (BarEquationNode)mathNode.AddChild(EquationNodeType.Bar);
            
            // Imposta la posizione della barra su Top
            barNode.BarPosition = EquationCharacterPositionType.Top;

            // Aggiungi contenuto base per la barra
            EquationNode baseNode = barNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Salva la cartella di lavoro
            workbook.Save("BarEquationDemo.xlsx");

            // Verifica il file salvato
            Workbook verifyWorkbook = new Workbook("BarEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            BarEquationNode verifyBarNode = (BarEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            Console.WriteLine("Bar Position: " + verifyBarNode.BarPosition);
            Console.WriteLine("Base Content: " + ((TextRunEquationNode)verifyBarNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Vedi anche

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


