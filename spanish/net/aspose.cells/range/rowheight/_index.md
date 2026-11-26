---
title: "Range.RowHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Establece o obtiene la altura de las filas en este rango"
type: docs
url: /es/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Establece u obtiene la altura de las filas en este rango

```csharp
public double RowHeight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos datos en la primera fila
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // Obtener la altura inicial de la fila
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // Ajustar automáticamente la fila
            worksheet.AutoFitRow(0);

            // Obtener la nueva altura de la fila después del ajuste automático
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // Establecer manualmente una nueva altura de fila
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


