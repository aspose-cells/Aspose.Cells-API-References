---
title: "WorkbookSettings.WindowLeftCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetri"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetro.

```csharp
public double WindowLeftCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà WindowLeftCM (distanza dal bordo sinistro dello schermo in centimetri)
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // Verifica l'impostazione stampandola
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // Salva la cartella di lavoro
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


