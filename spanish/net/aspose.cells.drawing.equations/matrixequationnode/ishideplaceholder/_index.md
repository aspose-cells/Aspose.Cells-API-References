---
title: "MatrixEquationNode.IsHidePlaceholder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad de MatrixEquationNode. Este atributo especifica la propiedad Ocultar Marcadores de Posición en una matriz. Cuando esta propiedad está activada, los marcadores de posición no aparecen en la matriz. Por defecto, los marcadores de posición sí aparecen, de modo que las ubicaciones donde se puede insertar texto son visibles"
type: docs
url: /es/net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

Este atributo especifica la propiedad Ocultar Marcadores de posición en una matriz. Cuando esta propiedad está activada, los marcadores de posición no aparecen en la matriz. Por defecto, los marcadores de posición sí aparecen de modo que las ubicaciones donde se puede insertar texto sean visibles.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Ejemplos

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
            
            // Agregar forma de ecuación
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener nodo matemático y agregar matriz
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Establecer propiedades de la matriz
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true; // Demonstrate IsHidePlaceholder property

            // Agregar matriz 2x2 con 1 en la diagonal
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

            // Guardar y verificar
            string outputPath = "MatrixEquationWithHiddenPlaceholder.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation created with IsHidePlaceholder=true. File saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


