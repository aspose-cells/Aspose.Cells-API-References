---
title: "Klass SystemTimeInterruptMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SystemTimeInterruptMonitor-klass. Enkelt implementering av AbstractInterruptMonitor genom att kontrollera och jämföra aktuell systemtid med användarspecificerad gräns"
type: docs
url: /sv/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

Enkel implementering av [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) genom att kontrollera och jämföra aktuell systemtid med användarspecificerad gräns.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Skapar en avbrottsmonitor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | Denna implementering kontrollerar bara om tidskostnaden (från det att monitorn startades till nu) är större än den användarspecificerade gränsen. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | Se [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Denna egenskap specificeras av användaren när denna monitorinstans konstrueras. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Startar monitorn med den angivna tidsgränsen. Starttiden för att beräkna tidskostnaden är exakt när denna metod anropas, så proceduren som ska övervakas bör startas omedelbart efter detta anrop. |

### Anmärkningar

Denna implementering är bara en enkel lösning för enkla scenarier. Den måste ofta hämta och kontrollera systemtiden, så den kan ha en viss negativ inverkan på prestandan.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // Skapa en instans av SystemTimeInterruptMonitor med terminateWithoutException satt till false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Skapa LoadOptions och sätt InterruptMonitor till den skapade monitorn
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Starta övervakning med en tidsgräns på 1000 millisekunder (1 sekund)
            monitor.StartMonitor(1000);

            try
            {
                // Läs in en arbetsbok med de angivna LoadOptions
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Om tidsåtgången för att läsa in mallfilen överstiger en sekund krävs avbrott och ett undantag kommer att kastas här
                // Annars, starta övervakning av spara‑proceduren med en ny tidsgräns
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Spara arbetsboken
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


