---
title: "WorkbookSettings.WindowWidthInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La larghezza della finestra in unità di pollice"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

La larghezza della finestra, in unità di pollice.

```csharp
public double WindowWidthInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta la larghezza della finestra in pollici
            settings.WindowWidthInch = 10.5;

            // Visualizza la larghezza della finestra in pollici
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // Salva la cartella di lavoro
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


