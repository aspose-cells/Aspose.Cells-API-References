---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale"
type: docs
url: /it/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;
            
            // Nascondi la barra di scorrimento orizzontale
            settings.IsHScrollBarVisible = false;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


