---
title: "Timeline.HeightPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Timeline. Devuelve o establece la altura de la línea de tiempo especificada en píxeles"
type: docs
url: /es/net/aspose.cells.timelines/timeline/heightpixel/
---
## Timeline.HeightPixel property

Devuelve o establece la altura de la línea de tiempo especificada, en píxeles.

```csharp
[Obsolete("Use Shape.Height property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int HeightPixel { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Height. Esta propiedad será eliminada 12 meses después a partir de mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyHeightPixelDemo
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
            sheet.Cells["A4"].Value = new DateTime(2023, 3, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregar línea de tiempo
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Establecer propiedades de la línea de tiempo incluyendo HeightPixel
            timeline.HeightPixel = 150;
            timeline.WidthPixel = 300;
            timeline.Caption = "Sales Timeline";

            // Guarda el libro de trabajo
            workbook.Save("TimelineHeightPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


