---
title: "WorkbookSettings.Author"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta l'autore del file"
type: docs
url: /it/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

Ottiene e imposta l'autore del file.

```csharp
public string Author { get; set; }
```

### Osservazioni

Non è impostato, controlla prima [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/) , poi controlla l'utente di Environment.

### Esempi

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Imposta la proprietà author
            settings.Author = "John Doe";

            // Aggiungi alcuni dati di esempio per dimostrare la funzionalità della cartella di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // Salva la cartella di lavoro
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


