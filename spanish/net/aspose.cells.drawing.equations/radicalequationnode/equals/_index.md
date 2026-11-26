---
title: "RadicalEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método RadicalEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/radicalequationnode/equals/
---
## RadicalEquationNode.Equals method

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

    public class RadicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Crea dos instancias de RadicalEquationNode
                RadicalEquationNode node1 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
                RadicalEquationNode node2 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));

                // Establece diferentes propiedades para demostrar la comparación de igualdad
                node1.IsDegHide = true;
                node2.IsDegHide = false;

                // Comparar los nodos usando el método Equals
                bool areEqual = node1.Equals(node2);

                // Mostrar el resultado de la comparación
                Console.WriteLine($"Are nodes equal? {areEqual}");

                // Compara con el mismo objeto
                areEqual = node1.Equals(node1);
                Console.WriteLine($"Are node1 and itself equal? {areEqual}");

                // Comparar con null
                areEqual = node1.Equals(null);
                Console.WriteLine($"Are node1 and null equal? {areEqual}");
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

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


