---
title: "Timeline.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Timeline. Devuelve o establece el nombre de la línea de tiempo especificada"
type: docs
url: /es/net/aspose.cells.timelines/timeline/name/
---
## Timeline.Name property

Devuelve o establece el nombre de la Línea de tiempo especificada

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelinePropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la línea de tiempo
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            sheet.Cells["A3"].PutValue(DateTime.Now);
            sheet.Cells["A4"].PutValue(DateTime.Now.AddDays(1));
            
            // Agregar una tabla dinámica que se usará como fuente de datos para la línea de tiempo
            sheet.Cells["C1"].PutValue("Pivot Table");
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Agregar una línea de tiempo usando la tabla dinámica
            int timelineIndex = sheet.Timelines.Add(pivotTable, 0, 0, "Timeline1");
            Aspose.Cells.Timelines.Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Establecer y demostrar la propiedad Name
            timeline.Name = "MyTimeline";
            Console.WriteLine("Timeline name: " + timeline.Name);
        }
    }
}
```

### Ver también

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


