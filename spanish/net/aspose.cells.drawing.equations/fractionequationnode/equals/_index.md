---
title: "FractionEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FractionEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Dado que FractionEquationNode no tiene un constructor sin parámetros,
                // Demostraremos Equals con objetos que presumiblemente provienen de otro lugar en la API
                // Para propósitos de demostración, asumiremos que tenemos dos instancias para comparar
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // Comparar los objetos usando Equals
                bool areEqual = node1.Equals(node2);

                // Mostrar el resultado de la comparación
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // Comparar con null
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Comparar consigo mismo
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // Método auxiliar para simular la obtención de instancias de FractionEquationNode
        // (En uso real, estos provendrían de la API)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // Esto es solo un marcador de posición; en realidad obtendrías estos de la API
            // Por ejemplo: worksheet.Equations.AddFractionEquationNode() o similar
            return null; // Actual implementation would depend on API
        }
    }
}
```

### Ver también

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


