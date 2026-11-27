---
title: "Worksheet.PivotTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Hämtar alla pivot‑tabeller i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Hämtar alla pivottabeller i detta arbetsblad.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Exempel

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till pivot‑tabellsamlingen från kalkylbladet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Kontrollera om det finns några pivot‑tabeller
            if (pivotTables.Count > 0)
            {
                // Hämta den första pivot‑tabellen
                PivotTable pivotTable = pivotTables[0];
                
                // Rensa eventuella befintliga filter
                pivotTable.PivotFilters.Clear();
                
                // Uppdatera pivot‑tabellens data
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // Spara den modifierade arbetsboken
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### Se även

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


