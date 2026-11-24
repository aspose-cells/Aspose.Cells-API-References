---
title: "WorkbookSettings.WindowTopInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters in Zoll."
type: docs
url: /de/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zoll.

```csharp
public double WindowTopInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;

            // Setze die WindowTopInch-Eigenschaft, um das Fenster 2 Zoll vom oberen Rand zu positionieren
            settings.WindowTopInch = 2.0;

            // Überprüfe die Einstellung, indem du sie ausgibst
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // Speichere die Arbeitsmappe
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


