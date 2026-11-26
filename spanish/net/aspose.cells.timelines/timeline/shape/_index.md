---
title: "Timeline.Shape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Timeline. Devuelve el objeto TimelineShape asociado a esta línea de tiempo"
type: docs
url: /es/net/aspose.cells.timelines/timeline/shape/
---
## Timeline.Shape property

Devuelve el objeto [`TimelineShape`](../../../aspose.cells.drawing/timelineshape/) asociado a esta línea de tiempo.

```csharp
public TimelineShape Shape { get; }
```

### Ejemplos

```csharp
using System;
using System.Reflection;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyShapeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos mínimos requeridos para una línea de tiempo (campo de fecha)
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = DateTime.Now.AddDays(-2);
            sheet.Cells["A3"].Value = DateTime.Now.AddDays(-1);
            sheet.Cells["A4"].Value = DateTime.Now;

            try
            {
                // Crear una tabla dinámica que servirá como fuente de datos de la línea de tiempo
                int pivotIdx = sheet.PivotTables.Add("A1:A4", "C1", "PivotTable1");
                PivotTable pivot = sheet.PivotTables[pivotIdx];
                pivot.AddFieldToArea(PivotFieldType.Row, "Date");
                pivot.RefreshData();

                // Agregar una línea de tiempo vinculada a la tabla dinámica
                int timelineIdx = sheet.Timelines.Add(pivot, 0, 0, "Date");
                Timeline timeline = sheet.Timelines[timelineIdx];

                // Intentar leer la propiedad 'Shape' mediante reflexión (si existe en esta versión)
                PropertyInfo shapeProp = typeof(Timeline).GetProperty("Shape", BindingFlags.Public | BindingFlags.Instance);
                if (shapeProp != null)
                {
                    object shapeValue = shapeProp.GetValue(timeline);
                    Console.WriteLine("Shape property value: " + (shapeValue ?? "null"));
                }
                else
                {
                    Console.WriteLine("The Timeline class does not expose a 'Shape' property in this version.");
                }

                // Guarde el libro de trabajo para verificar que la creación de la línea de tiempo se haya completado con éxito
                workbook.Save("TimelineShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [TimelineShape](../../../aspose.cells.drawing/timelineshape/)
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


