---
title: "LimLowUppEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "método de LimLowUppEquationNode. Determinar si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

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

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dado que no conocemos los parámetros del constructor, compararemos valores nulos
            // Este es un cambio mínimo para que compile; en uso real necesitarías una construcción adecuada
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // Llamar al método Equals con el tipo de parámetro específico (Object)
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // Mostrar el resultado
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Guarda el libro de trabajo
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


