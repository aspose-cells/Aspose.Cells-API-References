---
title: "MathematicalEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método MathematicalEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Cree dos instancias de MathematicalEquationNode para comparación
                // Dado que MathematicalEquationNode no tiene un constructor sin parámetros,
                // necesitaremos pasar null o los parámetros apropiados
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // Comparar los nodos usando el método Equals
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Mostrar el resultado de la comparación
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Comparar con un tipo de objeto diferente
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


