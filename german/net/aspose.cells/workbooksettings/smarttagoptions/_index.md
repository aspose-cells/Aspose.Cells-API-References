---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Ruft die Optionen des SmartTag ab"
type: docs
url: /de/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Liest die Optionen des Smart‑Tags.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();

                // Greifen Sie auf die Arbeitsmappeneinstellungen zu
                WorkbookSettings settings = workbook.Settings;

                // Lese die SmartTagOptions-Eigenschaft
                var smartTagOptions = settings.SmartTagOptions;

                // Zeige Informationen über die SmartTagOptions-Instanz an
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // Optional kannst du den Standardzustand über ToString() inspizieren
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Speichere die Arbeitsmappe (die Datei enthält die Standardeinstellungen)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


