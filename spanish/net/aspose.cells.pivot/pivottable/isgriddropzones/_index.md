---
title: "PivotTable.IsGridDropZones"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si el informe de PivotTable muestra el diseño clásico de tabla dinámica. permite arrastrar campos en la cuadrícula"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/isgriddropzones/
---
## PivotTable.IsGridDropZones property

Indica si el informe de PivotTable muestra el diseño clásico de tabla dinámica. (permite arrastrar campos en la cuadrícula)

```csharp
public bool IsGridDropZones { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsGridDropZonesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Agregar tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Establecer la propiedad IsGridDropZones
            pivotTable.IsGridDropZones = true;
            Console.WriteLine("IsGridDropZones: " + pivotTable.IsGridDropZones);

            // Guarda el libro de trabajo
            workbook.Save("PivotTable_IsGridDropZones_Example.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


