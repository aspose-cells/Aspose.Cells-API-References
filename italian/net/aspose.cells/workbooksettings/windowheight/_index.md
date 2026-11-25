---
title: "WorkbookSettings.WindowHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. L'altezza della finestra in unità di punto"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

L'altezza della finestra, in unità di punto.

```csharp
public double WindowHeight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Imposta la proprietà WindowHeight
            settings.WindowHeight = 600;
            
            // Verifica il valore di WindowHeight
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
            // Salva la cartella di lavoro
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


