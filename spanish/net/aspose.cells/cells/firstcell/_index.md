---
title: "Cells.FirstCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene la primera celda en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Obtiene la primera celda en esta hoja de cálculo.

```csharp
public Cell FirstCell { get; }
```

### Observaciones

Devuelve null si no hay datos en la hoja de cálculo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class CellsPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(2000);
            
            // Obtener colección de celdas
            Cells cells = worksheet.Cells;
            
            // Demostrar la propiedad FirstCell
            Cell firstCell = cells.FirstCell;
            Console.WriteLine($"First cell address: {firstCell.Name}");
            Console.WriteLine($"First cell value: {firstCell.Value}");
            
            // Crear gráfico usando FirstCell y LastCell
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
            chart.ShowLegend = true;
            
            // Guarda el libro de trabajo
            workbook.Save("FirstCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


