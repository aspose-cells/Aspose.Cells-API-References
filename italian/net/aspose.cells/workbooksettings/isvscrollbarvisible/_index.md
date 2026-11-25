---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale"
type: docs
url: /it/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;
            
            // Nascondi la barra di scorrimento verticale
            settings.IsVScrollBarVisible = false;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


