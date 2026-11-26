---
title: "HorizontalPageBreak.StartColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HorizontalPageBreak. Obtiene el índice de columna inicial de este salto de página horizontal"
type: docs
url: /es/net/aspose.cells/horizontalpagebreak/startcolumn/
---
## HorizontalPageBreak.StartColumn property

Obtiene el índice de columna inicial de este salto de página horizontal.

```csharp
public int StartColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyStartColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue saltos de página en diferentes columnas para demostrar StartColumn
            int index1 = worksheet.HorizontalPageBreaks.Add("Y30");
            int index2 = worksheet.HorizontalPageBreaks.Add("B30");
            
            HorizontalPageBreak hPageBreak1 = worksheet.HorizontalPageBreaks[index1];
            HorizontalPageBreak hPageBreak2 = worksheet.HorizontalPageBreaks[index2];
            
            Console.WriteLine($"First Break Start Column: {hPageBreak1.StartColumn}");
            Console.WriteLine($"Second Break Start Column: {hPageBreak2.StartColumn}");
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


