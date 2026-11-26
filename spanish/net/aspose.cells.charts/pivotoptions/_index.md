---
title: "Clase PivotOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.PivotOptions class. Representa un tipo complejo que especifica los controles pivot que aparecen en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

Representa un tipo complejo que especifica los controles pivot que aparecen en el gráfico

```csharp
public class PivotOptions
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | Especifica si un control para cada campo de PivotTable en el eje de filas de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | Especifica si un control para cada campo de PivotTable en el eje de datos de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | Especifica si un control para cada campo de PivotTable en el eje de página de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | Especifica si un control para cada campo de PivotTable en el eje de columnas de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Especifica si algún control pivot puede aparecer en el gráfico pivot. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar los botones de expandir o contraer campos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotOptionsDemo
    {
        public static void PivotOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos para la tabla pivot.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Agregar una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Accede a los PivotOptions del gráfico.
            PivotOptions pivotOptions = chart.PivotOptions;

            // Establece propiedades de PivotOptions.
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Guarda el libro de trabajo
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


