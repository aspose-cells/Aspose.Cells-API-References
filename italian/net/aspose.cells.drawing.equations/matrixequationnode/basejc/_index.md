---
title: "MatrixEquationNode.BaseJc"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MatrixEquationNode. Questo attributo specifica l'allineamento della matrice. Il testo al di fuori della matrice può essere allineato con il fondo, la parte superiore o il centro di una funzione matrice. Per impostazione predefinita la matrice assume l'allineamento al centro"
type: docs
url: /it/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

Questo attributo specifica l'allineamento della matrice. Il testo al di fuori della matrice può essere allineato in basso, in alto o al centro di una funzione matrice. Per impostazione predefinita, la matrice assume l'allineamento al centro.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyBaseJcDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma di equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il paragrafo dell'equazione e aggiungi un nodo matrice
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Imposta le proprietà della matrice includendo BaseJc
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Aggiungi il contenuto della matrice 2x2 (matrice identità)
            for (int row = 0; row < 2; row++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Salva la cartella di lavoro
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### Vedi anche

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


