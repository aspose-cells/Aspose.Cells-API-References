---
title: "Classe InterruptMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.InterruptMonitor. Représente tous les opérateurs concernant l'interruption"
type: docs
url: /fr/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Représente tous les opérateurs concernant l'interruption.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Marquez le moniteur comme demandant une interruption |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Lorsque la procédure est interrompue, indique s'il faut terminer la procédure silencieusement ou lancer une Exception. La valeur par défaut est false, c'est‑à‑dire que lorsque [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) est true, une [`CellsException`](../cellsexception/) avec le code Interrupted sera levée. (Héritée de [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Interrompez l'opérateur actuel. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Créez et assignez le moniteur d'interruption
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simulez l'interruption de l'opération
                monitor.Interrupt();
                
                // Essayez d'enregistrer (devrait être interrompu)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Save completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted.");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### Voir aussi

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


