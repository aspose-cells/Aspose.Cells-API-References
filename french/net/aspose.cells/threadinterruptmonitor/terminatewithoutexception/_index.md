---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadInterruptMonitor. Voir TerminateWithoutException. Cette propriété est spécifiée par l'utilisateur lors de la construction de cette instance de moniteur."
type: docs
url: /fr/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

Voir [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). Cette propriété est spécifiée par l'utilisateur lors de la construction de cette instance de moniteur.

```csharp
public override bool TerminateWithoutException { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de ThreadInterruptMonitor avec la valeur initiale de TerminateWithoutException
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // Affichez la valeur actuelle de la propriété
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Démarrez la surveillance avec une limite de 5 secondes
            monitor.StartMonitor(5000);

            // Démontrer le traitement qui pourrait être interrompu
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // Simuler un traitement long
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Processing was interrupted");
                        break;
                    }
                    worksheet.Cells[i, 0].Value = "Value " + i;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception occurred: " + ex.Message);
            }
            finally
            {
                monitor.FinishMonitor();
            }

            // Créer un autre moniteur avec TerminateWithoutException défini sur true
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // Enregistrer le résultat
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


