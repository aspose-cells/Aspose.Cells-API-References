---
title: "EquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método EquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationnode/equals/
---
## EquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos nodos de ecuación para comparación
            EquationNode node1 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            EquationNode node2 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

            try
            {
                // Llamar al método Equals con parámetro Object
                bool areEqual = node1.Equals((object)node2);

                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Modificar node2 para que sean diferentes
                node2.AddChild(EquationNodeType.Base);

                areEqual = node1.Equals((object)node2);
                Console.WriteLine($"After modification, are they equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            workbook.Save("EquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


