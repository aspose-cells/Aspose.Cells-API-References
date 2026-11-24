---
title: "IWarningCallback.Warning"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IWarningCallback-Methode. Unser Callback muss nur die Warning-Methode implementieren"
type: docs
url: /de/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

Unser Callback muss nur die Methode "Warning" implementieren.

```csharp
public void Warning(WarningInfo warningInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| warningInfo | WarningInfo | Warnungsinfo |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackMethodWarningWithWarningInfoDemo : IWarningCallback
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var demo = new IWarningCallbackMethodWarningWithWarningInfoDemo();
            workbook.Settings.WarningCallback = demo;

            try
            {
                Console.WriteLine("Warning callback is set up. Any warnings during operations will be displayed.");
                
                // Demonstrieren Sie die Wirkung, indem Sie mit einem potenziellen Warnungszenario speichern
                worksheet.Cells["A1"].Formula = "=1/0"; // This may trigger a warning
                workbook.Save("WarningDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning Type: {warningInfo.Type}");
            Console.WriteLine($"Description: {warningInfo.Description}");
            Console.WriteLine($"Corrected Object: {warningInfo.CorrectedObject ?? "null"}");
        }
    }
}
```

### Siehe auch

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


