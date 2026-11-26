---
title: "SparklineCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineCollection. Obtiene el elemento Sparkline en el índice especificado"
type: docs
url: /es/net/aspose.cells.charts/sparklinecollection/item/
---
## SparklineCollection indexer

Obtiene el elemento [`Sparkline`](../../sparkline/) en el índice especificado.

```csharp
public Sparkline this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);

            // Crear grupo de sparkline
            SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
            int idx = sparklineGroups.Add(SparklineType.Line, "A1:D1", false, CellArea.CreateCellArea(0, 4, 0, 4));
            SparklineGroup group = sparklineGroups[idx];

            // Acceda a los sparklines usando la propiedad Item
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline Data Range: " + sparkline.DataRange);
            Console.WriteLine("Sparkline Type: " + group.Type);

            // Modificar los datos del sparkline
            worksheet.Cells["A1"].PutValue(8);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


