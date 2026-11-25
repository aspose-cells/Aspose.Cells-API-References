---
title: "WorkbookSettings.WindowLeft"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorkbookSettings property. La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra in unità di punto"
type: docs
url: /it/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto.

```csharp
public double WindowLeft { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà WindowLeft per posizionare la finestra a 100 pixel dal lato sinistro
            settings.WindowLeft = 100;

            // Imposta altre proprietà della finestra per la dimostrazione
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // Aggiungi dati di esempio al foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // Salva la cartella di lavoro
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


