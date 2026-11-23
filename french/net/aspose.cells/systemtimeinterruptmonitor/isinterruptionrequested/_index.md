---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SystemTimeInterruptMonitor. Cette implémentation vérifie simplement si le coût temporel depuis le moment où ce moniteur a démarré jusqu'à maintenant dépasse la limite spécifiée par l'utilisateur."
type: docs
url: /fr/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de SystemTimeInterruptMonitor
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // Démarrer la surveillance avec une limite de temps de 5 secondes
            monitor.StartMonitor(5000);

            // Afficher la valeur initiale de IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Simuler une opération de longue durée
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // Vérifier si une interruption a été demandée
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // Afficher la valeur finale de IsInterruptionRequested
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Enregistrer le résultat
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


