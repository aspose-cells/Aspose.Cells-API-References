---
title: "WorkbookSettings.NumberGroupSeparator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorkbookSettings proprietà. Ottiene o imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. Il valore predefinito è il separatore di gruppo della regione corrente."
type: docs
url: /it/net/aspose.cells/workbooksettings/numbergroupseparator/
---
## WorkbookSettings.NumberGroupSeparator property

Ottiene o imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. Il valore predefinito è il separatore di gruppo della Regione corrente.

```csharp
public char NumberGroupSeparator { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberGroupSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            wb.Settings.NumberDecimalSeparator = ',';
            wb.Settings.NumberGroupSeparator = '.';
            
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00";
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(12345.6798);
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


