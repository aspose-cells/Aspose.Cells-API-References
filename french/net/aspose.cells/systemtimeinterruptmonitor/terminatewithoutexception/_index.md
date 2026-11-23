---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SystemTimeInterruptMonitor. Voir TerminateWithoutException. Cette propriété est spécifiée par l'utilisateur lors de la construction de cette instance de moniteur."
type: docs
url: /fr/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

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

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de SystemTimeInterruptMonitor avec la valeur initiale de TerminateWithoutException
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Afficher la valeur actuelle de la propriété TerminateWithoutException
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Démarrer la surveillance avec une limite de temps de 1000 ms
            monitor.StartMonitor(1000);

            // Démontrer l'effet de TerminateWithoutException en tentant une opération longue
            try
            {
                // Simuler une opération longue qui pourrait dépasser la limite de temps
                for (int i = 0; i < 100000; i++)
                {
                    worksheet.Cells[i, 0].Value = i;
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Operation interrupted by monitor");
                        break;
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception caught: " + ex.Message);
            }

            // Créer un autre moniteur avec TerminateWithoutException défini sur true
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // Enregistrez le classeur
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


