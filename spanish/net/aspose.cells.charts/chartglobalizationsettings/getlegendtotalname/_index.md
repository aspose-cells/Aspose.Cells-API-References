---
title: "ChartGlobalizationSettings.GetLegendTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartGlobalizationSettings. Obtiene el nombre del total para la leyenda"
type: docs
url: /es/net/aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/
---
## ChartGlobalizationSettings.GetLegendTotalName method

Obtiene el nombre de total para la leyenda

```csharp
public virtual string GetLegendTotalName()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crear configuraciones de globalización y obtener el nombre del total de la leyenda
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendTotalName = globalizationSettings.GetLegendTotalName();

            // Mostrar el resultado
            Console.WriteLine("Legend Total Name: " + legendTotalName);

            // Guardar el libro de trabajo
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


