---
title: "Klass ThreadInterruptMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ThreadInterruptMonitor‑klassen. En enkel implementation av AbstractInterruptMonitor genom att starta en annan tråd för att kräva avbrott efter att ha sovit i den av användaren angivna tidsgränsen"
type: docs
url: /sv/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Enkel implementation av [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) genom att starta en annan tråd för att kräva avbrott efter att ha sovit i den av användaren angivna tidsgränsen.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Skapar en avbrottsmonitor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | Denna implementering kontrollerar bara om tidskostnaden (från det att monitorn startades till nu) är större än den användarspecificerade gränsen. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | Se [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Denna egenskap specificeras av användaren när denna monitorinstans konstrueras. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Avslutar övervakaren för ett förfarande. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Startar monitorn med den angivna tidsgränsen. Starttiden för att beräkna tidskostnaden är exakt när denna metod anropas, så proceduren som ska övervakas bör startas omedelbart efter detta anrop. |

### Anmärkningar

En övervakningsinstans kan användas upprepade gånger, så länge du övervakar varje process i sekvens. Den bör inte användas för att övervaka flera förfaranden samtidigt i flera trådar.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // Skapa en instans av ThreadInterruptMonitor med terminateWithoutException satt till false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Skapa LoadOptions och sätt InterruptMonitor till den skapade monitorn
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Starta övervakaren med en tidsgräns på 1000 millisekunder (1 sekund)
            monitor.StartMonitor(1000);

            try
            {
                // Läs in en arbetsbok med de angivna LoadOptions
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Avsluta övervakaren för inläsningsproceduren
                monitor.FinishMonitor();

                // Starta övervakaren igen med en ny tidsgräns på 1500 millisekunder (1,5 sekunder)
                monitor.StartMonitor(1500);

                // Spara arbetsboken
                wb.Save("result.xlsx");

                // Avsluta övervakaren för sparningsproceduren
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


