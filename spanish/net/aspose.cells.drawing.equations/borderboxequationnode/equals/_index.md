---
title: "BorderBoxEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método BorderBoxEquationNode. Determinar si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/borderboxequationnode/equals/
---
## BorderBoxEquationNode.Equals method

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

    public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Crear dos instancias de BorderBoxEquationNode para comparación
                // Dado que BorderBoxEquationNode no tiene un constructor sin parámetros,
                // usaremos el constructor de la clase base (asumiendo que EquationNode pueda tener uno)
                BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                
                // Comparar los nodos usando el método Equals
                bool areEqual = node1.Equals((object)node2);
                
                // Mostrar el resultado de la comparación
                Console.WriteLine($"The nodes are equal: {areEqual}");
                
                // Comparar con un tipo de objeto diferente
                object differentObject = new object();
                bool areEqualWithDifferentType = node1.Equals(differentObject);
                Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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

* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


