---
title: "Timeline.LeftPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Timeline. Devuelve o establece el desplazamiento horizontal de la forma de la línea de tiempo desde su columna izquierda en píxeles"
type: docs
url: /es/net/aspose.cells.timelines/timeline/leftpixel/
---
## Timeline.LeftPixel property

Devuelve o establece el desplazamiento horizontal de la forma de la línea de tiempo desde su columna izquierda, en píxeles.

```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Left. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyLeftPixelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();

            // Agregue una línea de tiempo y obténgala de la colección
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Demostrar la propiedad LeftPixel
            timeline.LeftPixel = 150;
            timeline.TopPixel = 50;
            timeline.WidthPixel = 200;
            timeline.HeightPixel = 80;

            // Guardar el libro de trabajo
            workbook.Save("TimelineLeftPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


