---
title: "ChartGlobalizationSettings.GetAxisTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartGlobalizationSettings. Obtiene el nombre del título para el eje"
type: docs
url: /es/net/aspose.cells.charts/chartglobalizationsettings/getaxistitlename/
---
## ChartGlobalizationSettings.GetAxisTitleName method

Obtiene el nombre del título para el eje

```csharp
public virtual string GetAxisTitleName()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Crear configuraciones de globalización y obtener el nombre del título del eje
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string axisTitleName = globalizationSettings.GetAxisTitleName();

            // Establecer el título del eje
            chart.ValueAxis.Title.Text = axisTitleName;
            chart.CategoryAxis.Title.Text = axisTitleName;

            // Mostrar el nombre del título del eje
            Console.WriteLine("Axis Title Name: " + axisTitleName);

            // Guarda el libro de trabajo
            workbook.Save("ChartGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


