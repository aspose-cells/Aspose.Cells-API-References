---
title: "Chart.HidePivotFieldButtons"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart property. Indica si se ocultan los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart"
type: docs
url: /es/net/aspose.cells.charts/chart/hidepivotfieldbuttons/
---
## Chart.HidePivotFieldButtons property

Indica si se ocultan los botones de campo del gráfico dinámico solo cuando el gráfico es PivotChart.

```csharp
public bool HidePivotFieldButtons { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ChartPropertyHidePivotFieldButtonsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Demostrar la propiedad HidePivotFieldButtons
            chart.HidePivotFieldButtons = false; // Show pivot field buttons
            chart.RefreshPivotData();

            // Guarda el libro de trabajo
            workbook.Save("HidePivotFieldButtonsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


