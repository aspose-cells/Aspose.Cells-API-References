---
title: "TrendlineCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TrendlineCollection. Añade un objeto Trendline a esta colección con el tipo especificado"
type: docs
url: /es/net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Añade un objeto [`Trendline`](../../trendline/) a esta colección con el tipo especificado.

```csharp
public int Add(TrendlineType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | TrendlineType | Tipo de Trendline. |

### Valor de retorno

[`Trendline`](../../trendline/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["B4"].PutValue(8);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar datos de la serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Añadir línea de tendencia exponencial a la primera serie
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            // Guarda el libro de trabajo
            workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Añade un objeto [`Trendline`](../../trendline/) a esta colección con el tipo y nombre especificados.

```csharp
public int Add(TrendlineType type, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | TrendlineType | Tipo de Trendline. |
| name | String | Nombre de Trendline. |

### Valor de retorno

[`Trendline`](../../trendline/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Añadir serie y establecer datos
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].Name = "Data Series";

            // Añadir línea de tendencia con TrendlineType y nombre
            chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
            
            // Establecer algunas propiedades de Trendline
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            
            workbook.Save("TrendlineDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


