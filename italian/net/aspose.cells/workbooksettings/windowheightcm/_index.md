---
title: "WorkbookSettings.WindowHeightCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. L'altezza della finestra in unità di centimetro"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

L'altezza della finestra, in unità di centimetro.

```csharp
public double WindowHeightCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà WindowHeightCM
            settings.WindowHeightCM = 15.5;

            // Visualizza il valore impostato
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

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


