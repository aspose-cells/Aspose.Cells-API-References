---
title: "Range.UnionRanges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Devuelve el resultado de la unión de dos rangos"
type: docs
url: /es/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

Devuelve el resultado de la unión de dos rangos.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ranges | Range[] | El rango |

### Valor de retorno

La unión de dos rangos.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea datos de ejemplo en celdas
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // Crea rangos para unir
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // Llama a UnionRanges con el parámetro Range[]
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // Aplica estilo para mostrar el rango de unión
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


