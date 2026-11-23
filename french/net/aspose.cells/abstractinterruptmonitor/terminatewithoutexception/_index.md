---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractInterruptMonitor. Lorsque la procédure est interrompue, faut‑il terminer la procédure silencieusement ou lever une Exception. La valeur par défaut est false, c’est‑à‑dire que lorsque IsInterruptionRequested est true, une CellsException avec le code Interrupted sera levée."
type: docs
url: /fr/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

Lorsque la procédure est interrompue, faut‑il terminer la procédure silencieusement ou lever une Exception. La valeur par défaut est false, c’est‑à‑dire que lorsque [`IsInterruptionRequested`](../isinterruptionrequested/) est true, une [`CellsException`](../../cellsexception/) avec le code Interrupted sera levée.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir la feuille de calcul pour créer une charge de travail de traitement
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // Démontrer SystemTimeInterruptMonitor avec une terminaison par exception
            var interruptMonitor1 = new SystemTimeInterruptMonitor(terminateWithoutException: false);
            Console.WriteLine($"Initial TerminateWithoutException: {interruptMonitor1.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor1;
            interruptMonitor1.StartMonitor(1); // Set 1ms timeout

            try
            {
                workbook.Save("TerminateWithException.xlsx");
                Console.WriteLine("Saved successfully (unexpected with false setting)");
            }
            catch (CellsException ex)
            {
                Console.WriteLine($"Operation terminated with exception: {ex.Message}");
            }

            // Démontrer SystemTimeInterruptMonitor avec une terminaison silencieuse
            var interruptMonitor2 = new SystemTimeInterruptMonitor(terminateWithoutException: true);
            Console.WriteLine($"\nNew TerminateWithoutException: {interruptMonitor2.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor2;
            interruptMonitor2.StartMonitor(1);

            try
            {
                workbook.Save("TerminateSilently.xlsx");
                Console.WriteLine("Saved without exception (expected with true setting)");
            }
            catch (CellsException)
            {
                Console.WriteLine("Exception caught (unexpected with true setting)");
            }

        }
    }

}
```

### Voir aussi

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


