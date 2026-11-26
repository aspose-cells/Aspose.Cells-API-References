---
title: "Clase SlicerCacheItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Slicers.SlicerCacheItem. Representa el elemento de origen de datos del slicer"
type: docs
url: /es/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Representa el elemento de origen de datos del segmentador

```csharp
public class SlicerCacheItem
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | Especifica si el `SlicerCacheItem` está seleccionado o no. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Devuelve el texto de la etiqueta para el elemento del slicer. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheItemDemo
    {
        public static void Run()
        {
            // Cargar el libro de trabajo con slicer
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Obtener el primer slicer en el libro de trabajo
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Iterar a través de los elementos del caché de slicer
            Console.WriteLine("Slicer Cache Items:");
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
                Console.WriteLine($"Item {i}: Selected={slicerCacheItem.Selected}, Value={slicerCacheItem.Value}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


