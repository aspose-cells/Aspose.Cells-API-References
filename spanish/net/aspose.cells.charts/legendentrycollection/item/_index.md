---
title: "LegendEntryCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LegendEntryCollection. Obtiene el elemento LegendEntry en el índice especificado"
type: docs
url: /es/net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Obtiene el elemento [`LegendEntry`](../../legendentry/) en el índice especificado.

```csharp
public LegendEntry this[int index] { get; }
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
    public class LegendEntryCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Category 2");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Acceder a las entradas de la leyenda
            LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Demostrar el uso de la propiedad Item
            for (int i = 0; i < legendEntries.Count; i++)
            {
                LegendEntry entry = legendEntries[i];
                Console.WriteLine($"Legend Entry {i}:");
                Console.WriteLine($"- Font: {entry.Font.Name}");
                Console.WriteLine($"- Auto Scale Font: {entry.AutoScaleFont}");
            }

            // Modificar la primera entrada de la leyenda
            if (legendEntries.Count > 0)
            {
                legendEntries[0].Font.Name = "Arial";
                legendEntries[0].Font.Size = 12;
                legendEntries[0].AutoScaleFont = false;
            }
        }
    }
}
```

### Ver también

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


