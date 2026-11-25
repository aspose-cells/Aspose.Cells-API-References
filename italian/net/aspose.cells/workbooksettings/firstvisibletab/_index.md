---
title: "WorkbookSettings.FirstVisibleTab"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta la prima scheda del foglio di lavoro visibile"
type: docs
url: /it/net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

Ottiene o imposta la prima scheda del foglio di lavoro visibile.

```csharp
public int FirstVisibleTab { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFirstVisibleTabDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Imposta l'indice della prima scheda visibile (basato su 0)
            workbook.Settings.FirstVisibleTab = 1;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Verifica l'impostazione
            Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


