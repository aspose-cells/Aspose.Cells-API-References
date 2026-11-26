---
title: "BoxEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método BoxEquationNode. Determina si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dos objetos BoxEquationNode para compararlos
            // Dado que BoxEquationNode no tiene un constructor sin parámetros,
            // necesitaremos crearlos de manera diferente. Suponiendo que podamos obtenerlos de algún lugar,
            // o crearlos con algunos parámetros predeterminados.
            // Para propósitos de demostración, simplemente los declararemos y asignaremos null (aunque en código real necesitarías una inicialización adecuada)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // Llama al método Equals con los tipos de parámetro específicos (Object)
                    bool areEqual = node1.Equals(objToCompare);

                    // Mostrar el resultado
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // Agregar el resultado a la hoja de cálculo
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // Guardar el resultado
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


