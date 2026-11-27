---
title: "IWarningCallback.Warning"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IWarningCallback‑metod. Vår återuppringning behöver bara implementera Warning‑metoden"
type: docs
url: /sv/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

Vår återuppringning behöver bara implementera "Warning"-metoden.

```csharp
public void Warning(WarningInfo warningInfo)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| warningInfo | WarningInfo | varningsinformation |

### Exempel

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
                
                // Demonstrera effekten genom att spara med ett potentiellt varningsscenario
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

### Se även

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


