---
title: "PivotFilter.FilterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-egenskap. Hämtar filtertypen för pivottfiltret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/filtertype/
---
## PivotFilter.FilterType property

Hämtar filtertypen för pivotfiltret.

```csharp
public PivotFilterType FilterType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Få åtkomst till första kalkylbladet och pivottabellen
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Tillämpa värdefilter (mindre än 2) på första basfältet
            pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in arbetsboken igen för att verifiera filtret
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
            
            // Hämta det tillämpade filtret och demonstrera FilterType-egenskapen
            PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
            Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
        }
    }
}
```

### Se även

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


