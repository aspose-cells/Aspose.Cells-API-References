---
title: "Range.UnionRang"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Devuelve el resultado de la unión de dos rangos"
type: docs
url: /es/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

Devuelve el resultado de la unión de dos rangos.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | El rango |

### Valor de retorno

La unión de dos rangos.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método Range.UnionRanges(). Este método será eliminado 12 meses después desde mayo de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dos rangos para demostrar UnionRang
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // Establece algunos valores en los rangos para visualización
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // Llama al método UnionRang para combinar los dos rangos
                Range[] unionResult = range1.UnionRang(range2);

                // Muestra información sobre el resultado de la unión
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // Marca los rangos de unión con un borde para visualización
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


