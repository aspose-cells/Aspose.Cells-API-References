---
title: "Cells.StandardHeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt in Zoll"
type: docs
url: /de/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Liest oder legt die Standardzeilenhöhe in diesem Arbeitsblatt in Zoll fest.

```csharp
public double StandardHeightInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erhalte die Standardhöhe in Zoll
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // Setze eine neue Standardhöhe (1 Zoll)
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


