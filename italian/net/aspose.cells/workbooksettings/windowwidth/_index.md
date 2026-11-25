---
title: "WorkbookSettings.WindowWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La larghezza della finestra in unità di punto"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

La larghezza della finestra, in unità di punto.

```csharp
public double WindowWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Imposta la proprietà WindowWidth
            settings.WindowWidth = 800;
            
            // Verifica il valore di WindowWidth
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // Salva la cartella di lavoro
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


