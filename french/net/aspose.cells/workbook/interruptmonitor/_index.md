---
title: "Workbook.InterruptMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient et définit le moniteur d'interruption"
type: docs
url: /fr/net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Obtient et définit le moniteur d'interruption.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyInterruptMonitorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données à la feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Créez et assignez le moniteur d'interruption
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simuler une opération de longue durée en interrompant immédiatement
                monitor.Interrupt();
                
                // Tentative d'enregistrement - devrait être interrompue
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
                    Console.WriteLine($"Error occurred: {e.Message}");
                }
            }
        }
    }
}
```

### Voir aussi

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


