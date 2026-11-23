---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ThreadInterruptMonitor. Termine le moniteur pour une procédure"
type: docs
url: /fr/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Termine le moniteur pour une procédure.

```csharp
public void FinishMonitor()
```

### Remarques

Appeler cette méthode après la procédure surveillée peut libérer le thread du moniteur plus tôt, surtout lorsqu'il n'y a aucune interruption pour celle-ci (le coût temporel de cette procédure est inférieur à la limite de temps spécifiée).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // Créez une instance de ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Créer LoadOptions et définir l'InterruptMonitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Démarrer la surveillance avec un délai d'attente de 1 seconde
            monitor.StartMonitor(1000);

            try
            {
                // Simulez une opération de longue durée
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // Terminer la surveillance de l'opération
                monitor.FinishMonitor();
                Console.WriteLine("Operation completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


