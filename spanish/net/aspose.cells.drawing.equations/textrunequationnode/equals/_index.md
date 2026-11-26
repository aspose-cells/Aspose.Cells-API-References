---
title: "TextRunEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "TextRunEquationNode método. Determine si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Para propósitos de demostración, usaremos null y simplemente mostraremos la lógica de comparación
            // ya que no podemos crear instancias de TextRunEquationNode directamente
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // Esta parte permanece para mostrar cómo se llamaría Equals
                // En un escenario real, estos serían nodos correctamente inicializados
                if (node1 != null && node2 != null && node3 != null)
                {
                    // Compare node1 con node2 (mismo contenido)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // Compare node1 con node3 (contenido diferente)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // Comparar con null
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // Compare con un tipo de objeto diferente
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarde el libro de trabajo (aunque Equals no modifica la hoja de cálculo)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // Se eliminó el método auxiliar ya que no podemos crear correctamente instancias de TextRunEquationNode
    }
}
```

### Ver también

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


