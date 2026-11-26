---
title: "Slicer.SlicerCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Slicer. Devuelve el objeto SlicerCache asociado al slicer. Solo lectura."
type: docs
url: /es/net/aspose.cells.slicers/slicer/slicercache/
---
## Slicer.SlicerCache property

Devuelve el objeto SlicerCache asociado al segmentador. Solo lectura.

```csharp
public SlicerCache SlicerCache { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertySlicerCacheDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Crear una tabla a partir del rango de datos
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Agregar una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Agregar un segmentador
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Demostrar el uso de SlicerCache
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Name: " + slicerCache.Name);
            Console.WriteLine("Slicer Cache Source Name: " + slicerCache.SourceName);
            Console.WriteLine("Slicer Cache Items Count: " + slicerCache.SlicerCacheItems.Count);

            // Guarda el libro de trabajo
            workbook.Save("SlicerCacheDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SlicerCache](../../slicercache/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


