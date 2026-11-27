---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Anger om alla anslutningar ska uppdateras vid öppning av fil i MS Excel"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Anger om alla anslutningar ska uppdateras vid öppning av filen i MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsbladsamlingen
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Lägg till några exempel på kalkylblad
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // Ställ in IsRefreshAllConnections-egenskapen
            worksheets.IsRefreshAllConnections = true;
            
            // Visa det aktuella värdet för IsRefreshAllConnections
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Spara arbetsboken
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


