---
title: "WorksheetCollection.RefreshAll"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Uppdatera alla pivottabeller och diagram med pivottabellskälla"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

Uppdatera alla pivottabeller och diagram med pivottabellskälla.

```csharp
[Obsolete("Use Workbook.RefreshAll() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RefreshAll()
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Workbook.RefreshAll()-metoden. Denna metod kommer att tas bort 12 månader senare sedan april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshAllDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och formler
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Lägg till formler som kommer att uppdateras
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["C2"].PutValue("=SUM(B2:B3)");
            
            // Ändra några värden
            worksheet.Cells["B2"].PutValue(3.0);
            worksheet.Cells["B3"].PutValue(2.0);
            
            // Uppdatera alla formler i alla arbetsblad
            workbook.Worksheets.RefreshAll();
            
            // Skriv ut den uppdaterade totalen
            Console.WriteLine("Refreshed total: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


