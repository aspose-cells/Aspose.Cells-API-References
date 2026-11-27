---
title: "PivotFilter.GetTop10Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-metod. Hämtar topp 10-inställningen för filtret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

Hämtar top‑10-inställningen för filtret.

```csharp
public Top10Filter GetTop10Value()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Få åtkomst till första kalkylbladet och pivottabellen
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Tillämpa topp 10-filter på första basfältet (visa de 2 bästa objekten efter antal)
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Hämta det tillämpade filtret och dess topp 10-värde
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // Skriv ut filterdetaljerna
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


