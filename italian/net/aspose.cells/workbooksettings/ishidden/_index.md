---
title: "WorkbookSettings.IsHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se questa cartella di lavoro è nascosta"
type: docs
url: /it/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Indica se questa workbook è nascosta.

```csharp
public bool IsHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà IsHidden su true
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // Salva la cartella di lavoro
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // Crea un'altra cartella di lavoro
            Workbook workbook2 = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings2 = workbook2.Settings;

            // Imposta la proprietà IsHidden su false (predefinito)
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // Salva la cartella di lavoro
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // Carica e verifica le cartelle di lavoro salvate
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


