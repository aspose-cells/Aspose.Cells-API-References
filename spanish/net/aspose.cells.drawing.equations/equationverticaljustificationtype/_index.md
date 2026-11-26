---
title: "Enumeración EquationVerticalJustificationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.Equations.EquationVerticalJustificationType. Esto especifica la justificación vertical predeterminada de las ecuaciones en el documento"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationverticaljustificationtype/
---
## EquationVerticalJustificationType enumeration

Esto especifica la justificación vertical predeterminada de las ecuaciones en el documento.

```csharp
public enum EquationVerticalJustificationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Top | `0` | superior |
| Center | `1` | centrado |
| Bottom | `2` | inferior |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationVerticalJustificationTypeDemo
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

            // Establecer propiedades de la matriz
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Agregar filas y columnas de la matriz
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // Guarda el libro de trabajo
            string outputPath = "EquationVerticalJustificationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("File saved with vertical justification demo: " + outputPath);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


