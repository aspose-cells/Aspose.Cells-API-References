---
title: "WarningInfo.Description"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WarningInfo-Eigenschaft. Gibt die Beschreibung der Warninformation zurück"
type: docs
url: /de/net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

Beschreibung der Warnungsinfo abrufen.

```csharp
public string Description { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyDescriptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen doppelten definierten Namen, um eine Warnung auszulösen
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning

            // Abrufen des Warn-Callbacks
            WarningCallback callback = new WarningCallback();
            workbook.Settings.WarningCallback = callback; // Correct property path

            // Speichern, um die Warnung auszulösen
            workbook.Save("output.xlsx");

            // Demonstrieren Sie die Verwendung der Description-Eigenschaft
            if (callback.LastWarning != null)
            {
                Console.WriteLine("Warning Description: " + callback.LastWarning.Description);
                Console.WriteLine("Warning Type: " + callback.LastWarning.Type);
            }
        }
    }

    public class WarningCallback : IWarningCallback
    {
        public WarningInfo LastWarning { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            LastWarning = warningInfo;
        }
    }
}
```

### Siehe auch

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


