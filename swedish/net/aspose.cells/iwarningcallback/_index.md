---
title: "Gränssnitt IWarningCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IWarningCallback-gränssnitt. Återuppringningsgränssnitt för varning"
type: docs
url: /sv/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

Återuppringningsgränssnitt för varning.

```csharp
public interface IWarningCallback
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Vår återuppringning behöver bara implementera "Warning"-metoden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // Implementering av Warning-metoden från IWarningCallback-gränssnittet
        public void Warning(WarningInfo warningInfo)
        {
            // Visa varningsmeddelandet
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in varningsåteruppringning
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Läs in en arbetsbok med potentiella varningar
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Spara arbetsboken
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


