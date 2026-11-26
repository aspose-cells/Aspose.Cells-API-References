---
title: "ReferredArea.EndColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. La columna final del área"
type: docs
url: /es/net/aspose.cells/referredarea/endcolumn/
---
## ReferredArea.EndColumn property

La columna final del área.

```csharp
public int EndColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyEndColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Cell cell = worksheet.Cells["B2"];
            cell.Formula = "=SUM(A1:C3)";
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            foreach (ReferredArea area in referredAreas)
            {
                Console.WriteLine($"StartColumn: {area.StartColumn}");
                Console.WriteLine($"EndColumn: {area.EndColumn}");
                Console.WriteLine($"Columns spanned: {area.EndColumn - area.StartColumn + 1}");
            }
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


