---
title: "Legend.LegendEntries"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Legend. Obtiene una colección de todos los objetos LegendEntry en la leyenda del gráfico especificado. No se admite establecer las entradas de leyenda del gráfico de superficie. Por lo tanto, devolverá null si el tipo de gráfico es de superficie."
type: docs
url: /es/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Obtiene una colección de todos los objetos LegendEntry en la leyenda del gráfico especificado. No se admite establecer las entradas de leyenda del gráfico de superficie. Por lo tanto, devolverá null si el tipo de gráfico es de superficie.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Acceder a las entradas de la leyenda
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Eliminar la segunda entrada de leyenda
            legendEntries[1].IsDeleted = true;
            
            // Guarda el libro de trabajo
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


