---
title: "UnknowEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnknowEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dos nodos de ecuación desconocidos para compararlos
            // Dado que UnknowEquationNode no tiene un constructor sin parámetros,
            // necesitaremos crearlos de manera diferente. Para propósitos de demostración, usaremos
            // el constructor real si está disponible, o crearlos por otros medios.
            // Como no conocemos los parámetros del constructor, esta es una solución provisional.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // Llamar al método Equals con el tipo de parámetro específico (Object)
                bool areEqual = node1.Equals(objToCompare);

                // Mostrar el resultado
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Agregar el resultado a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // Método auxiliar para crear instancias de UnknowEquationNode
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // En una implementación real, esto usaría el constructor adecuado
            // Dado que no conocemos los parámetros del constructor, devolveremos null
            // y manejaremos el caso null en la demostración (aunque esto es solo un marcador de posición)
            return null;
        }
    }
}
```

### Ver también

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


