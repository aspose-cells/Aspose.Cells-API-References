---
title: "HorizontalPageBreak.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HorizontalPageBreak. Obtiene el índice de fila basado en cero"
type: docs
url: /es/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Obtiene el índice de fila basado en cero.

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue saltos de página horizontales
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // Obtenga la colección de saltos de página horizontales
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // Muestre los números de fila de los saltos de página
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


