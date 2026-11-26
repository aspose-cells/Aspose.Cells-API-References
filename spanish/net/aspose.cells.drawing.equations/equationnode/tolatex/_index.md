---
title: "EquationNode.ToLaTeX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Convierte esta ecuación a una expresión LaTeX"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

Convertir esta ecuación a expresión LaTeX.

```csharp
public string ToLaTeX()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToLaTeXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para contener la ecuación
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Obtener el nodo de ecuación
            var equationNode = shape.GetEquationParagraph();

            // Crear una ecuación de fracción simple
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // Llamar al método ToLaTeX
                string latexExpression = equationNode.ToLaTeX();
                
                // Mostrar el resultado
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // Agregar la salida LaTeX a una celda
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


