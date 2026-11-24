---
title: "WorkbookSettings.RemovePersonalInformation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings property. Wahr, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können"
type: docs
url: /de/net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

Wahr, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze RemovePersonalInformation auf true
            workbook.Settings.RemovePersonalInformation = true;
            
            // Fügen Sie einige Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Email");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue("john@example.com");
            
            // Speichere die Arbeitsmappe
            string outputPath = "output_with_personal_info_removed.xlsx";
            workbook.Save(outputPath);
            
            // Lade die gespeicherte Arbeitsmappe, um die Einstellung zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("RemovePersonalInformation setting: " + 
                loadedWorkbook.Settings.RemovePersonalInformation);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


