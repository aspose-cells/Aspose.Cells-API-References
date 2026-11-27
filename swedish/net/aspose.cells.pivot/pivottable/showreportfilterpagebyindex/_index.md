---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Visa alla rapportfilter-sidor enligt positionsindexet i PageFields"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

Visa alla rapportfilter‑sidor enligt positionsindexet i PageFields.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| posIndex | Int32 | Positionsindexet i PageFields |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // Kom åt det första kalkylbladet som innehåller pivottabellen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Visa rapportfilter-sidor efter index (position) för sidfältet
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // Spara arbetsboken
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


