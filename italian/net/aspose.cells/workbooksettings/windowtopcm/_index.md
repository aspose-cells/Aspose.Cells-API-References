---
title: "WorkbookSettings.WindowTopCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La distanza dal bordo superiore dell'area client al bordo superiore della finestra in unità di centimetri"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro.

```csharp
public double WindowTopCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà WindowTopCM (posizione dall'alto in centimetri)
            settings.WindowTopCM = 2.5;

            // Visualizza il valore corrente di WindowTopCM
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // Salva la cartella di lavoro
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


