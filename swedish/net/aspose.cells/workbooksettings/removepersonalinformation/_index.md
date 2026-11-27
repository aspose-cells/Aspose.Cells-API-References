---
title: "WorkbookSettings.RemovePersonalInformation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Sant om personlig information kan tas bort från den angivna arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

Sant om personlig information kan tas bort från den angivna arbetsboken.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in RemovePersonalInformation till sant
            workbook.Settings.RemovePersonalInformation = true;
            
            // Lägg till lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Email");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue("john@example.com");
            
            // Spara arbetsboken
            string outputPath = "output_with_personal_info_removed.xlsx";
            workbook.Save(outputPath);
            
            // Läs in den sparade arbetsboken för att verifiera inställningen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("RemovePersonalInformation setting: " + 
                loadedWorkbook.Settings.RemovePersonalInformation);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


