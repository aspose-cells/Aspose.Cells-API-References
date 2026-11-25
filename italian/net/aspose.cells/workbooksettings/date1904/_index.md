---
title: "WorkbookSettings.Date1904"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta un valore che indica se la cartella di lavoro utilizza il sistema di data 1904"
type: docs
url: /it/net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Ottiene o imposta un valore che indica se la workbook utilizza il sistema di data 1904.

```csharp
public bool Date1904 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDate1904Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Date1904 = true;

            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Dimostra il tempo negativo con Date1904
            Style style = cell.GetStyle();
            style.Custom = "h:mm";
            cell.SetStyle(style);
            cell.PutValue(-0.0736111111111112);
            Console.WriteLine("Negative time value: " + cell.DisplayStringValue);

            // Dimostra la data negativa con Date1904
            style = cell.GetStyle();
            style.Custom = "mm/dd/yyyy h:mm:ss";
            cell.SetStyle(style);
            cell.PutValue(-42389.47075706);
            Console.WriteLine("Negative date value: " + cell.DisplayStringValue);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


