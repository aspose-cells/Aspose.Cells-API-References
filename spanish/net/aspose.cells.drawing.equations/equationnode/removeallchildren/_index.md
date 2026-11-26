---
title: "EquationNode.RemoveAllChildren"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Elimina todos los nodos hijos del nodo actual"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/removeallchildren/
---
## EquationNode.RemoveAllChildren method

Elimina todos los nodos hijos del nodo actual.

```csharp
public void RemoveAllChildren()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveAllChildrenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para contener la ecuación
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Obtener el nodo de ecuación
            var equationNode = ((TextBox)shape).GetEquationParagraph();

            // Añade algunos nodos hijos a la ecuación
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            numerator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            denominator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML

            Console.WriteLine($"Equation before RemoveAllChildren: {equationNode.ToMathML()}");

            try
            {
                // Llama al método RemoveAllChildren
                equationNode.RemoveAllChildren();

                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Equation after RemoveAllChildren: {equationNode.ToMathML()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAllChildren method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("EquationNodeMethodRemoveAllChildrenDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


