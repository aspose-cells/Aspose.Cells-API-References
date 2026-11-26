---
title: "SlicerCache.List"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SlicerCache. Indica si el segmentador asociado con la caché de segmentador especificada se basa en una fuente de datos NonOLAP"
type: docs
url: /es/net/aspose.cells.slicers/slicercache/list/
---
## SlicerCache.List property

Indica si el slicer asociado con el caché de slicer especificado se basa en una fuente de datos No-OLAP.

```csharp
public bool List { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyListDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Crear tabla con sobrecarga correcta
            int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Agregar slicer
            int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
            Slicer slicer = sheet.Slicers[slicerIdx];

            // Acceder a la caché de segmentador
            SlicerCache cache = slicer.SlicerCache;

            // Demostrar el uso de la propiedad List
            Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
        }
    }
}
```

### Ver también

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


