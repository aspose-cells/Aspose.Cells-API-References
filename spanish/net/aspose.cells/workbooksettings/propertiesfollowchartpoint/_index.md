---
title: "WorkbookSettings.PropertiesFollowChartPoint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si las propiedades de los puntos de datos y las etiquetas de datos en todos los gráficos de este libro de trabajo siguen su referencia"
type: docs
url: /es/net/aspose.cells/workbooksettings/propertiesfollowchartpoint/
---
## WorkbookSettings.PropertiesFollowChartPoint property

Indica si las propiedades de los puntos de datos y las etiquetas de datos en todos los gráficos de este workbook siguen su referencia.

```csharp
public bool PropertiesFollowChartPoint { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPropertiesFollowChartPointDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establezca PropertiesFollowChartPoint en true
            workbook.Settings.PropertiesFollowChartPoint = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verifique que la configuración se haya guardado
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("PropertiesFollowChartPoint: " + loadedWorkbook.Settings.PropertiesFollowChartPoint);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


