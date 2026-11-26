---
title: "Worksheet.AddPageBreaks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Agrega salto de página"
type: docs
url: /es/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Agrega un salto de página.

```csharp
public void AddPageBreaks(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar salto de página horizontal en la fila 1 (B2)
            worksheet.AddPageBreaks("B2");

            // Agregar salto de página horizontal en la fila 9 (B10)
            worksheet.AddPageBreaks("B10");

            // Verificar que el primer salto de página se agregó en la fila 1
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


