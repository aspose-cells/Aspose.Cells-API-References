---
title: "TickLabels.DisplayNumberFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Obtiene y establece el formato numérico de visualización de las etiquetas de marcas"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/displaynumberformat/
---
## TickLabels.DisplayNumberFormat property

Obtiene y establece el formato numérico de visualización de las etiquetas de marcas.

```csharp
public string DisplayNumberFormat { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDisplayNumberFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A2:A3", true);
            chart.NSeries.CategoryData = "B2:B3";
            
            // Establecer formato numérico a través de la propiedad NumberFormat en su lugar
            chart.CategoryAxis.TickLabels.NumberFormat = "m/d/yyyy";
            chart.ValueAxis.TickLabels.NumberFormat = "#,##0";
            
            // Guarda el libro de trabajo
            workbook.Save("TickLabelsDisplayNumberFormatDemo.xlsx");
            
            Console.WriteLine("DisplayNumberFormat for CategoryAxis: " + 
                chart.CategoryAxis.TickLabels.DisplayNumberFormat);
            Console.WriteLine("DisplayNumberFormat for ValueAxis: " + 
                chart.ValueAxis.TickLabels.DisplayNumberFormat);
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


