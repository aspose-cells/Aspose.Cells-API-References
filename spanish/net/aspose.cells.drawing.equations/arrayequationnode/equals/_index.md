---
title: "ArrayEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ArrayEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/arrayequationnode/equals/
---
## ArrayEquationNode.Equals method

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

    public class ArrayEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos nodos de ecuación de matriz
            ArrayEquationNode arrayEquation1 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);
            ArrayEquationNode arrayEquation2 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);

            // Agregar nodos hijos para que sean diferentes
            EquationNode child1 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation1);
            // Usar ToLaTeX() o ToMathML() en lugar de la propiedad Value
            arrayEquation1.AddChild(child1);

            EquationNode child2 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation2);
            arrayEquation2.AddChild(child2);

            try
            {
                // Llamar al método Equals con objetos diferentes
                bool result1 = arrayEquation1.Equals(arrayEquation2);
                Console.WriteLine($"Comparing different array equations: {result1}");

                // Llamar a Equals con el mismo objeto
                bool result2 = arrayEquation1.Equals(arrayEquation1);
                Console.WriteLine($"Comparing same array equation: {result2}");

                // Llamar a Equals con null
                bool result4 = arrayEquation1.Equals(null);
                Console.WriteLine($"Comparing with null: {result4}");
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ArrayEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ArrayEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


