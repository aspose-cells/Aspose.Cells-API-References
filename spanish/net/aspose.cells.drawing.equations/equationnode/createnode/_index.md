---
title: "EquationNode.CreateNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Crea un nodo del tipo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

Crear un nodo del tipo especificado.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| equationType | EquationNodeType | Tipos de nodos de ecuación |
| libro de trabajo | Libro de trabajo | El objeto workbook asociado con la ecuación |
| padre | EquationNode | El nodo padre donde se encuentra este nodo |

### Valor de retorno

Si el tipo especificado existe, se devuelve el nodo correspondiente, y si el tipo no existe, se devuelve un nodo de tipo desconocido.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de ecuación
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Crea un nodo padre (fracción)
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // Crea nodos de numerador y denominador
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // Añade la fracción creada a la ecuación principal
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // Muestra la ecuación en una celda
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


