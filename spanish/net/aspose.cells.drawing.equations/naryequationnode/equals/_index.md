---
title: "NaryEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método NaryEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/naryequationnode/equals/
---
## NaryEquationNode.Equals method

Determinar si el nodo de ecuación actual es igual al nodo especificado

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El nodo especificado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para contener la ecuación
            var shape1 = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
            var equation1 = shape1.GetEquationParagraph();
            var naryNode1 = equation1.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode1 = (NaryEquationNode)naryNode1;
            naryEquationNode1.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Crear una segunda forma idéntica
            var shape2 = worksheet.Shapes.AddEquation(0, 100, 200, 50, 200, 50);
            var equation2 = shape2.GetEquationParagraph();
            var naryNode2 = equation2.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode2 = (NaryEquationNode)naryNode2;
            naryEquationNode2.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Crear una tercera forma diferente
            var shape3 = worksheet.Shapes.AddEquation(0, 200, 200, 50, 200, 50);
            var equation3 = shape3.GetEquationParagraph();
            var naryNode3 = equation3.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode3 = (NaryEquationNode)naryNode3;
            naryEquationNode3.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            try
            {
                // Comparar nodos idénticos
                bool result1 = naryEquationNode1.Equals(naryEquationNode2);
                Console.WriteLine($"Comparing identical nodes: {result1}");

                // Comparar nodos diferentes
                bool result2 = naryEquationNode1.Equals(naryEquationNode3);
                Console.WriteLine($"Comparing different nodes: {result2}");

                // Comparar con null
                bool result3 = naryEquationNode1.Equals(null);
                Console.WriteLine($"Comparing with null: {result3}");

                // Compare con un tipo de objeto diferente
                bool result4 = naryEquationNode1.Equals("string object");
                Console.WriteLine($"Comparing with different type: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("NaryEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


