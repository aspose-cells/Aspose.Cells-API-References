---
title: "EquationNode.ToMathML"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Convierte esta ecuación a expresión MathML"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/tomathml/
---
## EquationNode.ToMathML method

Convertir esta ecuación a expresión MathML.

```csharp
public string ToMathML()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToMathMLDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de ecuación - se añadieron los parámetros de ancho (300) y altura (100)
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
            var equation = shape.GetEquationParagraph();

            // Construir una ecuación simple: (a+b)^2 = a^2 + 2ab + b^2
            var equationNode = equation.AddChild(EquationNodeType.Text);
            var textNode = equationNode as TextRunEquationNode;
            textNode.Text = "(";

            var variableA = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableA.Text = "a";

            var plus = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            plus.Text = "+";

            var variableB = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableB.Text = "b";

            var closeParen = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            closeParen.Text = ")";

            var superscript = equation.AddChild(EquationNodeType.Superscript);
            var baseNode = superscript.AddChild(EquationNodeType.Base);
            var baseText = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            baseText.Text = "2";

            try
            {
                // Convertir la ecuación a MathML
                string mathML = equation.ToMathML();

                // Mostrar el MathML en la consola
                Console.WriteLine("MathML Output:");
                Console.WriteLine(mathML);

                // Escribir el MathML en una celda
                worksheet.Cells["A1"].PutValue("MathML Representation:");
                worksheet.Cells["A2"].PutValue(mathML);
                // Cambiado de worksheet.Cells.AutoFitColumns() a:
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting to MathML: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("EquationToMathMLDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


