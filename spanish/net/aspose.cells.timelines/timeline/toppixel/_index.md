---
title: "Timeline.TopPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Timeline. Devuelve o establece el desplazamiento vertical de la forma de la línea de tiempo desde su fila superior en píxeles"
type: docs
url: /es/net/aspose.cells.timelines/timeline/toppixel/
---
## Timeline.TopPixel property

Devuelve o establece el desplazamiento vertical de la forma de la línea de tiempo desde su fila superior, en píxeles.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Top. Esta propiedad será eliminada 12 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyTopPixelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellene datos de ejemplo
            cells["A1"].Value = "Date";
            cells["A2"].Value = new DateTime(2023, 1, 1);
            cells["A3"].Value = new DateTime(2023, 2, 1);
            cells["A4"].Value = new DateTime(2023, 3, 1);
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Agregar tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Agregar línea de tiempo
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];

            // Establecer propiedades de la línea de tiempo incluyendo TopPixel
            timeline.TopPixel = 50;
            timeline.HeightPixel = 100;
            timeline.WidthPixel = 300;

            // Guarda el libro de trabajo
            book.Save("TimelineTopPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


