---
title: "ReferredArea.EndColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReferredArea property. La colonne de fin de la zone"
type: docs
url: /fr/net/aspose.cells/referredarea/endcolumn/
---
## ReferredArea.EndColumn property

La colonne de fin de la zone.

```csharp
public int EndColumn { get; }
```

### Exemples

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

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


