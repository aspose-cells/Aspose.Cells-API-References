---
title: "InterruptMonitor.Interrupt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode InterruptMonitor. Interrompre l'opérateur actuel"
type: docs
url: /fr/net/aspose.cells/interruptmonitor/interrupt/
---
## InterruptMonitor.Interrupt method

Interrompez l'opérateur actuel.

```csharp
public void Interrupt()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InterruptMonitorMethodInterruptDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données à la feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 10000; i++)
            {
                worksheet.Cells[i, 0].Value = "Data " + i;
            }

            // Créer et définir le moniteur d'interruption
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            try
            {
                Console.WriteLine("Starting long operation...");
                
                // Simuler une opération longue dans un autre thread
                System.Threading.ThreadPool.QueueUserWorkItem(_ => 
                {
                    System.Threading.Thread.Sleep(1000); // Wait 1 second
                    Console.WriteLine("Interrupting operation...");
                    monitor.Interrupt(); // Call interrupt
                });

                // Effectuer une opération longue (sauvegarde)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Operation completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was interrupted successfully.");
                }
                else
                {
                    Console.WriteLine("Error: " + e.Message);
                }
            }
        }
    }
}
```

### Voir aussi

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


