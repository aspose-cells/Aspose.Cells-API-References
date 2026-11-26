---
title: "ChartGlobalizationSettings.GetAxisUnitName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartGlobalizationSettings. Obtiene el nombre de la unidad del eje"
type: docs
url: /es/net/aspose.cells.charts/chartglobalizationsettings/getaxisunitname/
---
## ChartGlobalizationSettings.GetAxisUnitName method

Obtiene el nombre de la unidad del eje

```csharp
public virtual string GetAxisUnitName(DisplayUnitType type)
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
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
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crear configuraciones de globalización y obtener el nombre de la unidad del eje
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string thousandsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);
            string millionsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Millions);

            // Mostrar resultados
            Console.WriteLine("Thousands unit name: " + thousandsUnit);
            Console.WriteLine("Millions unit name: " + millionsUnit);

            // Guardar el libro de trabajo
            workbook.Save("AxisUnitNameDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [DisplayUnitType](../../displayunittype/)
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


