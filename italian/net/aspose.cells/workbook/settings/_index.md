---
title: "Workbook.Settings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Rappresenta le impostazioni del workbook"
type: docs
url: /it/net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Rappresenta le impostazioni del workbook.

```csharp
public WorkbookSettings Settings { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertySettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi e modifica le impostazioni
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 30;
            workbook.Settings.FormulaSettings.MaxChange = 0.1;

            // Verifica le impostazioni
            Console.WriteLine("Iterative Calculation Enabled: " + 
                workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + 
                workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + 
                workbook.Settings.FormulaSettings.MaxChange);

            // Salva la cartella di lavoro
            workbook.Save("WorkbookSettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


