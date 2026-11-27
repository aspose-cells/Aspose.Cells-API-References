---
title: "WorkbookSettings.UpdateLinksType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Hämtar och anger hur externa länkar uppdateras när arbetsboken öppnas"
type: docs
url: /sv/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Hämtar och anger hur externa länkar uppdateras när arbetsboken öppnas.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Sätt UpdateLinksType till Never
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera inställningen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Skriv ut UpdateLinksType-värdet
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### Se även

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


