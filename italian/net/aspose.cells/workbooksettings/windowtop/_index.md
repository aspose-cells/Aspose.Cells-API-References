---
title: "WorkbookSettings.WindowTop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La distanza dal bordo superiore dell'area client al bordo superiore della finestra in unità di punto"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto.

```csharp
public double WindowTop { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Impostare la proprietà WindowTop per posizionare la finestra a 100 pixel dall'alto
            settings.WindowTop = 100;
            
            // Verificare il valore di WindowTop
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Salva la cartella di lavoro
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


