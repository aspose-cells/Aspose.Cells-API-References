---
title: "Enumeración DisplayUnitType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Charts.DisplayUnitType. Representa el tipo de unidad de visualización del eje de los gráficos"
type: docs
url: /es/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

Representa el tipo de unidad de visualización del eje del gráfico.

```csharp
public enum DisplayUnitType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | La unidad de visualización es Ninguna. |
| Hundreds | `1` | Especifica que los valores del gráfico se dividirán por 100. |
| Thousands | `2` | Especifica que los valores del gráfico se dividirán por 1,000. |
| TenThousands | `3` | Especifica que los valores del gráfico se dividirán por 10,000. |
| HundredThousands | `4` | Especifica que los valores del gráfico se dividirán por 100,000. |
| Millions | `5` | Especifica que los valores del gráfico se dividirán por 1,000,000. |
| TenMillions | `6` | Especifica que los valores del gráfico se dividirán por 10,000,000. |
| HundredMillions | `7` | Especifica que los valores del gráfico se dividirán por 100,000,000. |
| Billions | `8` | Especifica que los valores del gráfico se dividirán por 1,000,000,000. |
| Trillions | `9` | Especifica que los valores del gráfico se dividirán por 1,000,000,000,000. |
| Percentage | `10` | Los valores del gráfico se dividirán por 0.01. |
| Cust | `11` | Especifica un valor personalizado para la unidad de visualización. |
| Custom | `12` | Especifica un valor personalizado para la unidad de visualización. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una nueva hoja de cálculo al libro
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agrega NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Establecer la unidad de visualización del eje de valores a Millones
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Opcionalmente, mostrar la etiqueta de la unidad de visualización
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Guarda el libro de trabajo
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


