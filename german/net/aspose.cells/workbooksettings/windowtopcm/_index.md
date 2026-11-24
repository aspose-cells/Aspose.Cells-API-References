---
title: "WorkbookSettings.WindowTopCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Der Abstand vom oberen Rand des Clientbereichs bis zum oberen Rand des Fensters in Zentimetern."
type: docs
url: /de/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zentimeter.

```csharp
public double WindowTopCM { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Setze die WindowTopCM-Eigenschaft (Position von oben in Zentimetern).
            settings.WindowTopCM = 2.5;

            // Zeige den aktuellen WindowTopCM-Wert an.
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // Speichere die Arbeitsmappe
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


