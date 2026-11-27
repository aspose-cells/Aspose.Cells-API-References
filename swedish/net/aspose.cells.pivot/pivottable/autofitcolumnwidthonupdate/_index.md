---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om kolumnbredden ska anpassas automatiskt vid uppdatering"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Anger om kolumnbredden ska anpassas automatiskt vid uppdatering

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Kom åt kalkylbladet som innehåller pivottabellen
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // Kom åt pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Inaktivera automatisk anpassning av kolumnbredd vid uppdatering
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // Uppdatera pivottabellen för att tillämpa ändringarna
            worksheet.RefreshPivotTables();
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


