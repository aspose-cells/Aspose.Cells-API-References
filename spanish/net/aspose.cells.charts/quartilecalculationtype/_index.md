---
title: "Enumeración QuartileCalculationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.QuartileCalculationType enum. Representa los métodos de cálculo de cuartiles"
type: docs
url: /es/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

Representa los métodos de cálculo de cuartiles.

```csharp
public enum QuartileCalculationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Exclusive | `0` | El cálculo de cuartiles incluye la mediana al dividir el conjunto de datos en cuartiles. |
| Inclusive | `1` | El cálculo de cuartiles excluye la mediana al dividir el conjunto de datos en cuartiles. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series al gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Accede a las propiedades de diseño de la serie
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Establece el tipo de cálculo de cuartiles
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Guarda el libro de trabajo
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


