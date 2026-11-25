---
title: "WorkbookSettings.UpdateLinksType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta come vengono aggiornati i collegamenti esterni quando la cartella di lavoro viene aperta"
type: docs
url: /it/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Ottiene e imposta come aggiornare i collegamenti esterni quando la cartella di lavoro viene aperta.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta UpdateLinksType su Never
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare l'impostazione
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Restituisci il valore di UpdateLinksType
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### Vedi anche

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


