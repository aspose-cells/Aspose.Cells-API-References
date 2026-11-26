---
title: "BarEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método BarEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dos instancias de BarEquationNode para compararlas
            // Nota: La creación real de BarEquationNode dependería de los métodos de fábrica de la API
            // Para la demostración, asumiremos que estas son instancias correctamente inicializadas
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // Compara node1 con node2 (debería ser igual)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // Compara node1 con node3 (no debería ser igual)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // Compara node1 con null
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // Compara node1 con un tipo de objeto diferente
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // Método auxiliar para demostrar la obtención de un BarEquationNode
        // En un uso real, deberías usar el método API adecuado para crear estos
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // Esto es solo un marcador de posición - la implementación real dependería de la API
            // Por ejemplo, podría crearse a través de un objeto padre o un método de fábrica
            return null; // Replace with actual creation code
        }
    }
}
```

### Ver también

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


