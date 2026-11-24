---
title: "WorkbookSettings.WindowLeftCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Der Abstand vom linken Rand des Clientbereichs bis zum linken Rand des Fensters. In Zentimetern."
type: docs
url: /de/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters, gemessen in Zentimetern.

```csharp
public double WindowLeftCM { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;

            // Setze die WindowLeftCM-Eigenschaft (Abstand vom linken Rand des Bildschirms in Zentimetern).
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // Überprüfe die Einstellung, indem du sie ausgibst
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // Speichere die Arbeitsmappe
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


