---
title: "TimelineCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TimelineCollection. Obtiene el Timeline por índice"
type: docs
url: /es/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

Obtiene el Timeline por índice.

```csharp
public Timeline this[int index] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // Crear tabla dinámica primero
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Agregar timeline a la hoja de cálculo
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // Acceder al timeline usando la propiedad Item por índice
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // Demostrar el uso del timeline
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### Ver también

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

Obtiene el Timeline por el nombre del Timeline.

```csharp
public Timeline this[string name] { get; }
```

### Ejemplos

```csharp

[C#]

//Obtener el Timeline por el nombre del Timeline.
Timeline objByName = sheet.Timelines["date"];
```

### Ver también

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


