---
title: "WorkbookSettings.WindowTopInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La distanza dal bordo superiore dell'area client al bordo superiore della finestra in unità di pollice"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice.

```csharp
public double WindowTopInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà WindowTopInch per posizionare la finestra a 2 pollici dall'alto
            settings.WindowTopInch = 2.0;

            // Verifica l'impostazione stampandola
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // Salva la cartella di lavoro
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


