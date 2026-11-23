---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur SystemTimeInterruptMonitor. Construit un moniteur d'interruption"
type: docs
url: /fr/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Construit un moniteur d'interruption.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
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
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Créer une instance avec terminateWithoutException défini sur false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Configurer les options de chargement avec le moniteur
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Démarrer la surveillance avec une limite de temps de 1 seconde
            monitor.StartMonitor(1000);

            try
            {
                // Tentative de chargement d'un classeur
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // Réinitialiser le moniteur pour l'opération d'enregistrement avec une limite de 1,5 seconde
                monitor.StartMonitor(1500);
                wb.Save("output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


