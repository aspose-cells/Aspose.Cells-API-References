---
title: "Enumeración GradientPresetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.GradientPresetType. Representa el tipo de color predefinido de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

Representa el tipo de color preestablecido del degradado.

```csharp
public enum GradientPresetType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Brass | `0` | Color predefinido Bronce |
| CalmWater | `1` | Color predefinido Agua Tranquila |
| Chrome | `2` | Color predefinido Cromo |
| ChromeII | `3` | Color predefinido Cromo II |
| Daybreak | `4` | Color predefinido Amanecer |
| Desert | `5` | Color predefinido Desierto |
| EarlySunset | `6` | Color predefinido Atardecer Temprano |
| Fire | `7` | Color predefinido Fuego |
| Fog | `8` | Color predefinido Niebla |
| Gold | `9` | Color predefinido Oro |
| GoldII | `10` | Color predefinido Oro II |
| Horizon | `11` | Color predefinido Horizonte |
| LateSunset | `12` | Color predefinido Atardecer Tardío |
| Mahogany | `13` | Color predefinido Caoba |
| Moss | `14` | Color predefinido musgo |
| Nightfall | `15` | Color predefinido anochecer |
| Ocean | `16` | Color predefinido océano |
| Parchment | `17` | Color predefinido pergamino |
| Peacock | `18` | Color predefinido pavo real |
| Rainbow | `19` | Color predefinido arcoíris |
| RainbowII | `20` | Color predefinido arcoíris II |
| Sapphire | `21` | Color predefinido zafiro |
| Silver | `22` | Color predefinido plata |
| Wheat | `23` | Color predefinido trigo |
| Unknown | `24` | Color predefinido desconocido. Solo para el color predefinido (que no es igual a ningún color predefinido conocido) en el libro de trabajo de plantilla. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Acceder al eje de categorías del gráfico
            Axis categoryAxis = chart.CategoryAxis;

            // Acceder al formato de relleno del área del eje de categorías
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Establecer un color predefinido degradado para el formato de relleno
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Obtener el tipo de color predefinido degradado
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Guarda el libro de trabajo
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


