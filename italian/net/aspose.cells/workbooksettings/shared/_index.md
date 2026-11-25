---
title: "WorkbookSettings.Shared"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta un valore che indica se la cartella di lavoro è condivisa"
type: docs
url: /it/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Ottiene o imposta un valore che indica se il Workbook è condiviso.

```csharp
public bool Shared { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook book = new Workbook();
            
            // Imposta la proprietà Shared su true
            book.Settings.Shared = true;
            
            // Salva la cartella di lavoro
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // Carica la cartella di lavoro salvata per verificare la proprietà Shared
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


