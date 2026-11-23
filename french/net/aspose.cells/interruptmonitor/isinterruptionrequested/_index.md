---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété InterruptMonitor. Marquer le moniteur comme demandant une interruption"
type: docs
url: /fr/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

Marquez le moniteur comme demandant une interruption

```csharp
public override bool IsInterruptionRequested { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à sa première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un moniteur d'interruption et l'assigner au classeur
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Afficher l'état initial de IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // Simuler une opération de traitement de données de longue durée
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // Demander une interruption après le traitement de 500 lignes
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // Vérifier la demande d'interruption
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // Simuler le traitement des données
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // Enregistrer le classeur modifié
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### Voir aussi

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


