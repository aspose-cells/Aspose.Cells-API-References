---
title: "PivotTable.ShowReportFilterPage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Visa alla rapportsfilter-sidor enligt PivotField. PivotField måste vara placerad i PageFields."
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

Visa alla rapportfilter‑sidor enligt PivotField, PivotField måste vara placerad i PageFields.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageField | PivotField | PivotField-objektet |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("source.xlsx");
            
            // Få åtkomst till första kalkylbladet och pivottabellen
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Visa rapportsfilter-sidor för varje sidfält
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


