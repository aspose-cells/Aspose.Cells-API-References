---
title: "WorkbookSettings.Password"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings property. Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar"
type: docs
url: /de/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar.

```csharp
public string Password { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Daten hinzu
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // Setze das Passwort, um die Arbeitsmappe zu schützen
            wb.Settings.Password = "xixi";
            
            // Speichere die Arbeitsmappe
            wb.Save("output_with_password.ods");
            
            // Erstelle Ladeoptionen mit Passwort, um die geschützte Arbeitsmappe zu öffnen
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // Öffne die passwortgeschützte Arbeitsmappe
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // Überprüfe die Daten
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


