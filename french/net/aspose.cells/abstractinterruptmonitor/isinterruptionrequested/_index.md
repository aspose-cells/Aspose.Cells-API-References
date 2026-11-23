---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractInterruptMonitor. Indique si une interruption est demandée pour l'opération en cours. Si true, alors l'opération en cours sera interrompue. L'implémentation doit effectuer ici une vérification rapide et efficace, sinon cela pourrait devenir un autre goulot d'étranglement pour la procédure"
type: docs
url: /fr/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

Indique si une interruption est demandée pour l'opération en cours. Si true, alors l'opération en cours sera interrompue. L'implémentation doit effectuer ici une vérification rapide et efficace, sinon cela peut devenir un autre goulot d'étranglement pour la procédure.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;
    using System.Threading.Tasks;

    public class AbstractInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un moniteur d'interruption et l'assigner au classeur
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Afficher la valeur initiale
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Démarrer la tâche d’interruption
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // Simulation d’opération de longue durée
            Console.WriteLine("Starting data generation...");
            try
            {
                for (int i = 0; i < 500000000; i++)
                {
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine($"\nInterrupted at row {i}");
                        break;
                    }

                    worksheet.Cells[i, 0].Value = $"Data {i}";
                    
                    // Simuler le temps de traitement
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // Enregistrer le résultat
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### Voir aussi

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


