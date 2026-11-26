---
title: "Chart.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Obtiene o establece el tipo de gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/type/
---
## Chart.Type property

Obtiene o establece el tipo de un gráfico.

```csharp
public ChartType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de radar
            int chartIndex = sheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Chart type is: " + chart.Type);
            
            // Cambiar el tipo de gráfico a Columna
            chart.Type = ChartType.Column;
            Console.WriteLine("Chart type changed to: " + chart.Type);
        }
    }
}
```

### Ver también

* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


