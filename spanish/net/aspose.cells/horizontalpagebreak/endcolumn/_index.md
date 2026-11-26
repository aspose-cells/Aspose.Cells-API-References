---
title: "HorizontalPageBreak.EndColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HorizontalPageBreak. Obtiene el índice de columna final de este salto de página horizontal"
type: docs
url: /es/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Obtiene el índice de columna final de este salto de página horizontal.

```csharp
public int EndColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue un salto de página horizontal en la fila 5, que abarque desde la columna 2 hasta la 4
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // Muestre la propiedad EndColumn
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // Dado que EndColumn es de solo lectura, necesitamos eliminar y volver a agregar el salto de página para modificarlo
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### Ver también

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


