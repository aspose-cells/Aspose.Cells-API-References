---
title: "WorkbookSettings.WindowLeftInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollice"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowleftinch/
---
## WorkbookSettings.WindowLeftInch property

La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollice.

```csharp
public double WindowLeftInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà WindowLeftInch
            settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen

            // Aggiungi alcuni dati di esempio per dimostrare che la cartella di lavoro è funzionale
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");

            // Salva la cartella di lavoro
            workbook.Save("WindowLeftInchDemo.xlsx");

            Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


