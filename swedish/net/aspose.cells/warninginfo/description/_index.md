---
title: "WarningInfo.Description"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WarningInfo-egenskapen. Hämta beskrivning av varningsinformationen"
type: docs
url: /sv/net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

Hämta beskrivning av varningsinformation.

```csharp
public string Description { get; }
```

### Exempel

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

            // Skapa ett duplicerat definierat namn för att utlösa en varning
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning

            // Hämta varningscallback
            WarningCallback callback = new WarningCallback();
            workbook.Settings.WarningCallback = callback; // Correct property path

            // Spara för att utlösa en varning
            workbook.Save("output.xlsx");

            // Demonstrera användning av egenskapen Description
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

### Se även

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


