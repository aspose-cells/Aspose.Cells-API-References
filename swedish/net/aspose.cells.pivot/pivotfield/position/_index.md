---
title: "PivotField.Position"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Representerar indexet för PivotField i regionen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Representerar indexet för [`PivotField`](../) i regionen.

```csharp
public int Position { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPositionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // Få åtkomst till första kalkylbladet och dess pivottabell
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // Demonstrera användning av Position-egenskapen
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // Använd position för att visa rapportsfilter-sidor
            pt.ShowReportFilterPageByIndex(position);
            
            // Spara arbetsboken
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


