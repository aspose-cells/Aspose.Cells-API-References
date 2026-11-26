---
title: "Worksheet.Timelines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la colección de Timeline en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

Obtén la colección de Timeline en la hoja de cálculo

```csharp
public TimelineCollection Timelines { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTimelinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].Value = "Ship Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
            sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregar control de línea de tiempo para la tabla dinámica
            sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");

            // Guarda el libro de trabajo
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


