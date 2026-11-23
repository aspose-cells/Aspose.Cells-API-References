---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ThreadInterruptMonitor. Démarre le moniteur avec la limite de temps spécifiée. L'heure de début pour calculer le temps écoulé est simplement le moment où cette méthode est appelée, de sorte que la procédure à surveiller doit être lancée immédiatement après cet appel."
type: docs
url: /fr/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

Démarre le moniteur avec la limite de temps spécifiée. L'heure de départ pour calculer le temps écoulé est simplement le moment où cette méthode est appelée, ainsi la procédure à surveiller doit être lancée immédiatement après cet appel.

```csharp
public void StartMonitor(int msLimit)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| msLimit | Int32 | limite de temps (ms) pour déclencher l'interruption. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000);

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.FinishMonitor();

                monitor.StartMonitor(1500);
                wb.Save("result.xlsx");
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


