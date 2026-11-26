---
title: "SparklineGroupCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroupCollection. Obtiene el elemento SparklineGroup en el índice especificado"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Obtiene el elemento [`SparklineGroup`](../../sparklinegroup/) en el índice especificado.

```csharp
public SparklineGroup this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Agregar datos de ejemplo
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // Define el rango de datos y la ubicación para los sparklines
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // Agregar grupo de sparkline
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // Acceda al grupo de sparkline usando la propiedad Item
            SparklineGroup group = ws.SparklineGroups[index];
            
            // Personalice el sparkline
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Guarda el libro de trabajo
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


