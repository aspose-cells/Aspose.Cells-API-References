---
title: "WorkbookSettings.ShowTabs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta un valore che indica se le schede della cartella di lavoro sono visualizzate"
type: docs
url: /it/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

Ottiene o imposta un valore che indica se le schede del Workbook sono visualizzate.

```csharp
public bool ShowTabs { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Nascondi le schede del foglio di calcolo
            workbook.Settings.ShowTabs = false;
            
            // Salva la cartella di lavoro
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // Crea un'altra cartella di lavoro per mostrare le schede
            Workbook workbook2 = new Workbook();
            
            // Assicurati che le schede siano visibili (il valore predefinito è true)
            workbook2.Settings.ShowTabs = true;
            
            // Salva la cartella di lavoro
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


