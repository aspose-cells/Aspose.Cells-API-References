---
title: "WorkbookSettings.NumberDecimalSeparator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della regione corrente"
type: docs
url: /it/net/aspose.cells/workbooksettings/numberdecimalseparator/
---
## WorkbookSettings.NumberDecimalSeparator property

Ottiene o imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della Regione corrente.

```csharp
public char NumberDecimalSeparator { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberDecimalSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
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


