---
title: "Chart.ShowDataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart property. Obtiene o establece un valor que indica si el gráfico muestra una tabla de datos"
type: docs
url: /es/net/aspose.cells.charts/chart/showdatatable/
---
## Chart.ShowDataTable property

Obtiene o establece un valor que indica si el gráfico muestra una tabla de datos.

```csharp
public bool ShowDataTable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowDataTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            dataSheet.Cells["B1"].PutValue("Column 1");
            dataSheet.Cells["C1"].PutValue("Column 2");
            dataSheet.Cells["A2"].PutValue("Item 1");
            dataSheet.Cells["A3"].PutValue("Item 2");
            dataSheet.Cells["A4"].PutValue("Item 3");
            
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);
            dataSheet.Cells["C2"].PutValue(15);
            dataSheet.Cells["C3"].PutValue(25);
            dataSheet.Cells["C4"].PutValue(35);

            // Agregar hoja de gráfico
            int chartIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartIndex];
            
            // Crear gráfico
            chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = chartSheet.Charts[0];
            
            // Establecer origen de datos
            chart.NSeries.Add("Sheet1!B2:C4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";
            
            // Habilitar la visualización de la tabla de datos
            chart.ShowDataTable = true;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartWithDataTable.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


