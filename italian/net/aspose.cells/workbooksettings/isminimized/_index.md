---
title: "WorkbookSettings.IsMinimized"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorkbookSettings property. Rappresenta se il foglio di calcolo generato sarà aperto minimizzato"
type: docs
url: /it/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Rappresenta se il foglio di calcolo generato sarà aperto ridotto a icona.

```csharp
public bool IsMinimized { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta la proprietà IsMinimized su true
            workbook.Settings.IsMinimized = true;

            // Salva la cartella di lavoro
            workbook.Save("IsMinimizedDemo.xlsx");

            // Carica la cartella di lavoro salvata per verificare la proprietà
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // Visualizza il valore della proprietà IsMinimized
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


