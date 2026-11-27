---
title: "PivotField.Ungroup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Avgruppera pivottfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Avgruppera pivottfältet.

```csharp
public void Ungroup()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Avgruppera det första kolumnfältet
            pivotTable.ColumnFields[0].Ungroup();
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


