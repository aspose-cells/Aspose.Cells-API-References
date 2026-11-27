---
title: "Cells.IsDefaultRowHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskapen. Anger om raden är dold som standard"
type: docs
url: /sv/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Indikerar om raden är standarddolt.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in egenskapen för att dölja raden som standard
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // Visa det aktuella värdet för IsDefaultRowHidden
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


