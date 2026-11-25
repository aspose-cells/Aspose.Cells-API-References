---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MatrixEquationNode. Questo attributo specifica la proprietà Nascondi Segnaposti su una matrice. Quando questa proprietà è attiva i segnaposti non compaiono nella matrice. Per impostazione predefinita i segnaposti compaiono in modo che le posizioni dove è possibile inserire testo siano visibili"
type: docs
url: /it/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

Questo attributo specifica la proprietà Nascondi Segnaposti su una matrice. Quando questa proprietà è attiva, i segnaposti non compaiono nella matrice. Per impostazione predefinita, i segnaposti compaiono in modo che le posizioni dove è possibile inserire testo siano visibili.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class MatrixEquationNodePropertyIsHidePlaceholderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi forma dell'equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo matematico e aggiungi la matrice
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Imposta le proprietà della matrice
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // Aggiungi una matrice 2x2 con diagonale di 1
            for (int row = 0; row < 2; row++)
            {
                EquationNode matrixRow = matrixNode.AddChild(EquationNodeType.MatrixRow);
                for (int col = 0; col < 2; col++)
                {
                    EquationNode baseNode = matrixRow.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (row == col) ? "1" : "0";
                }
            }

            // Salva e verifica
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


