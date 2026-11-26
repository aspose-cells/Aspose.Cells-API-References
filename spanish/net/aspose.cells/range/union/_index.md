---
title: "Range.Union"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Devuelve la unión de dos rangos"
type: docs
url: /es/net/aspose.cells/range/union/
---
## Range.Union method

Devuelve la unión de dos rangos.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | El rango |

### Valor de retorno

La unión de dos rangos.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Range.UnionRanges(). Este método será eliminado 12 meses después desde noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree dos rangos para demostrar Union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // Rellene algunos datos en los rangos
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // Llame al método Union (nota: esta es la versión obsoleta)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // Muestre las direcciones de todos los rangos en la unión
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


