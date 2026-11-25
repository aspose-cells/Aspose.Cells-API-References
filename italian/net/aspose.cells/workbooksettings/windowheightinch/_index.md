---
title: "WorkbookSettings.WindowHeightInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. L'altezza della finestra in unità di pollice"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

L'altezza della finestra, in unità di pollice.

```csharp
public double WindowHeightInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta l'altezza della finestra in pollici
            settings.WindowHeightInch = 5.5;

            // Visualizza l'altezza della finestra in pollici
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // Salva la cartella di lavoro
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


