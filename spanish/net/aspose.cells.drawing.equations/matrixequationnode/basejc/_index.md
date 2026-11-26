---
title: "MatrixEquationNode.BaseJc"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad de MatrixEquationNode. Este atributo especifica la justificación de la matriz. El texto fuera de la matriz puede alinearse con la parte inferior, superior o el centro de una función de matriz. Por defecto, la matriz asume justificación centrada"
type: docs
url: /es/net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

Este atributo especifica la justificación de la matriz. El texto fuera de la matriz puede alinearse con la parte inferior, superior o el centro de una función de matriz. Por defecto, la matriz asume justificación centrada.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una forma de ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtener el párrafo de la ecuación y agregar un nodo de matriz
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Establecer propiedades de la matriz incluyendo BaseJc
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Agregar contenido de matriz 2x2 (matriz identidad)
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

            // Guarda el libro de trabajo
            string outputPath = "MatrixEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Matrix equation with BaseJc property demo completed.");
        }
    }
}
```

### Ver también

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


