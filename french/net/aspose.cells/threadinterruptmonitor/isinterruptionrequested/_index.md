---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadInterruptMonitor. Cette implémentation vérifie simplement si le temps écoulé depuis le démarrage de ce moniteur jusqu'à maintenant dépasse la limite spécifiée par l'utilisateur"
type: docs
url: /fr/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

Cette implémentation vérifie simplement si le temps écoulé (du moment où le moniteur a démarré jusqu'à maintenant) est supérieur à la limite spécifiée par l'utilisateur.

```csharp
public override bool IsInterruptionRequested { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // Démarrez la surveillance avec une limite de 2 secondes
            monitor.StartMonitor(2000);

            // Simulez une opération de longue durée
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // Vérifier si une interruption a été demandée
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // Simulez le travail
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // Terminez la surveillance
            monitor.FinishMonitor();

            // Enregistrer le résultat
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


