---
title: "Worksheet.CellWatches"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la colección de celdas en esta hoja de cálculo que están siendo observadas en la ventana de vigilancia"
type: docs
url: /es/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Obtiene la colección de celdas en esta hoja de cálculo que se están observando en la 'ventana de observación'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la celda B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Agregar vigilancia de celda para B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Mostrar información de vigilancia
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // Guarda el libro de trabajo
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


