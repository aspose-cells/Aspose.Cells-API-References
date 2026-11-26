---
title: "Clase SlicerCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Slicers.SlicerCache. Representa la descripción resumida del caché de slicer"
type: docs
url: /es/net/aspose.cells.slicers/slicercache/
---
## SlicerCache class

Representa la descripción resumida de la caché del segmentador

```csharp
public class SlicerCache
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CrossFilterType](../../aspose.cells.slicers/slicercache/crossfiltertype/) { get; set; } | (**Obsoleto.**) Indica cómo mostrar los elementos sin datos del slicer. |
| [List](../../aspose.cells.slicers/slicercache/list/) { get; } | Indica si el slicer asociado con el caché de slicer especificado se basa en una fuente de datos No-OLAP. |
| [Name](../../aspose.cells.slicers/slicercache/name/) { get; } | Devuelve el nombre del caché de slicer. |
| [SlicerCacheItems](../../aspose.cells.slicers/slicercache/slicercacheitems/) { get; } | Devuelve una colección SlicerCacheItem que contiene la colección de todos los elementos en el caché de slicer. Solo lectura |
| [SourceName](../../aspose.cells.slicers/slicercache/sourcename/) { get; } | Devuelve el nombre de este caché de slicer. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Crear datos de ejemplo
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";
            
            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;
            
            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;
            
            // Crear tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Agregar slicer y obtener su caché
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivot, "E12", "fruit");
            Slicer slicer = slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight2;
            
            // Demostrar el uso de SlicerCache
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Items:");
            foreach (SlicerCacheItem item in slicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            book.Save("out.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


