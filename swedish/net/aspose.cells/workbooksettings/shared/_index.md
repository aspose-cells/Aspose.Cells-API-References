---
title: "WorkbookSettings.Shared"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar eller anger ett värde som indikerar om Workbook är delad"
type: docs
url: /sv/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Hämtar eller anger ett värde som indikerar om arbetsboken är delad.

```csharp
public bool Shared { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook book = new Workbook();
            
            // Ställ in Shared-egenskapen till true
            book.Settings.Shared = true;
            
            // Spara arbetsboken
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // Läs in den sparade arbetsboken för att verifiera Shared-egenskapen
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


