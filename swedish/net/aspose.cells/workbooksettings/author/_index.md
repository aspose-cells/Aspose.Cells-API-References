---
title: "WorkbookSettings.Author"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar och anger författaren till filen"
type: docs
url: /sv/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

Hämtar och anger författaren till filen.

```csharp
public string Author { get; set; }
```

### Anmärkningar

Den är inte inställd, kontrollera först [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/), sedan kontrollera användaren i Environment.

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Ställ in författaregenskapen
            settings.Author = "John Doe";

            // Lägg till exempeldata för att demonstrera arbetsbokfunktionaliteten
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // Spara arbetsboken
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


