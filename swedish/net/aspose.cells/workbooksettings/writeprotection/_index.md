---
title: "WorkbookSettings.WriteProtection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Ger åtkomst till arbetsbokens skrivskyddsalternativ"
type: docs
url: /sv/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Tillhandahåller åtkomst till arbetsbokens skrivskyddsalternativ.

```csharp
public WriteProtection WriteProtection { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in skrivskyddsegenskaper
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // Spara arbetsboken
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Skriv ut skrivskyddsegenskaperna
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### Se även

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


