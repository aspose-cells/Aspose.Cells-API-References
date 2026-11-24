---
title: "WorkbookSettings.BuildVersion"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt die inkrementelle öffentliche Version der Anwendung an."
type: docs
url: /de/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Gibt die inkrementelle öffentliche Version der Anwendung an.

```csharp
public string BuildVersion { get; set; }
```

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;
            
            // Setze grundlegende Einstellungen.
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // Demonstriere die BuildVersion-Eigenschaft.
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


