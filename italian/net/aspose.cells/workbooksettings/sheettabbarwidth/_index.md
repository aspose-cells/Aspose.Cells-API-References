---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Larghezza della barra delle schede del foglio di lavoro in 1/1000 della larghezza della finestra"
type: docs
url: /it/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Impostare la proprietà SheetTabBarWidth
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // Ottenere e visualizzare il valore di SheetTabBarWidth
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


