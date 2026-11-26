---
title: "CellWatch.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellWatch. Obtiene y establece la columna de la celda"
type: docs
url: /es/net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

Obtiene y establece la columna de la celda.

```csharp
public int Column { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];
            
            Console.WriteLine("Initial Column: " + cellWatch.Column);
            
            cellWatch.Column = 1;
            Console.WriteLine("Modified Column: " + cellWatch.Column);
            
            workbook.Save("CellWatchColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


