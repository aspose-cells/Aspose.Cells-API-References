---
title: "WorkbookSettings.WindowWidthCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La larghezza della finestra in unità di centimetro"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

La larghezza della finestra, in unità di centimetro.

```csharp
public double WindowWidthCM { get; set; }
```

### Esempi

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Imposta la proprietà WindowWidthCM (20,32 cm = ~8 pollici)
            settings.WindowWidthCM = 20.32;
            
            // Verifica l'impostazione stampandola
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // Salva la cartella di lavoro
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


