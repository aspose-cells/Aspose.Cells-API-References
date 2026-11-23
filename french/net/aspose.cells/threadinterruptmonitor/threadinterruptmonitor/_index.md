---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur ThreadInterruptMonitor. Construit un moniteur d'interruption"
type: docs
url: /fr/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Construit un moniteur d'interruption.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer un ThreadInterruptMonitor avec throwOnInterrupted défini sur false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // Définir une courte limite de temps (100 ms) pour la démonstration
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // Effectuer une opération longue (sera interrompue)
                for (int i = 0; i < 100000; i++)
                {
                    workbook.Worksheets[0].Cells[i % 100, i / 100].PutValue(i);
                }
                
                Console.WriteLine("Operation completed without interruption");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### Voir aussi

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


