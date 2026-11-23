---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SystemTimeInterruptMonitor. Démarre le moniteur avec la limite de temps spécifiée. Le temps de départ pour calculer le coût temporel est simplement le moment où cette méthode est appelée, ainsi la procédure qui doit être surveillée doit être démarrée immédiatement après cet appel."
type: docs
url: /fr/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

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
    public class SystemTimeInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000); // 1 second time limit

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.StartMonitor(1500); // 1.5 second time limit
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

### Voir aussi

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


