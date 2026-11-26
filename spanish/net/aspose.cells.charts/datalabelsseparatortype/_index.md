---
title: "Enumeración DataLabelsSeparatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Charts.DataLabelsSeparatorType. Representa el tipo de separador de DataLabels"
type: docs
url: /es/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

Representa el tipo de separador de las etiquetas de datos.

```csharp
public enum DataLabelsSeparatorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Auto | `0` | Representa separador automático |
| Space | `1` | Representa espacio(" ") |
| Comma | `2` | Representa coma(",") |
| Semicolon | `3` | Representa un punto y coma(";") |
| Period | `4` | Representa punto(".") |
| NewLine | `5` | Representa salto de línea("\n") |
| Custom | `6` | Representa separador personalizado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos para el gráfico
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar la serie de datos al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a las DataLabels de la primera serie
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Establecer el tipo de separador a coma
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // Habilitar etiquetas de datos y establecer algunas propiedades
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // Establecer propiedades de fuente
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


