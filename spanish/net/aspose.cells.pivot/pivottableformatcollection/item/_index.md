---
title: "PivotTableFormatCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotTableFormatCollection propiedad. Obtiene el formato por el índice"
type: docs
url: /es/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Obtiene el formato por el índice.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");

            // Actualizar todas las tablas dinámicas
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // Accede a la primera tabla dinámica
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // Demostrar la propiedad Item accediendo al primer PivotFormat
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // Cambiar la configuración de formato usando la propiedad Item
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // Guardar el libro de trabajo modificado
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


