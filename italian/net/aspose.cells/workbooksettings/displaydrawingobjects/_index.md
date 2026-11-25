---
title: "WorkbookSettings.DisplayDrawingObjects"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se e come mostrare gli oggetti nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/displaydrawingobjects/
---
## WorkbookSettings.DisplayDrawingObjects property

Indica se e come mostrare gli oggetti nella workbook.

```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDisplayDrawingObjectsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Aggiungi una forma di esempio per dimostrare la proprietà
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta per visualizzare tutte le forme
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
            workbook.Save("DisplayShapes.xlsx");

            // Imposta per mostrare i segnaposto
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;
            workbook.Save("Placeholders.xlsx");

            // Imposta per nascondere tutte le forme
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
            workbook.Save("Hide.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


