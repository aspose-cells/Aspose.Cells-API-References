---
title: "WorkbookSettings.NumberDecimalSeparator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Ruft das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte ab oder legt es fest. Standard ist das Dezimaltrennzeichen der aktuellen Region"
type: docs
url: /de/net/aspose.cells/workbooksettings/numberdecimalseparator/
---
## WorkbookSettings.NumberDecimalSeparator property

Liest oder setzt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte. Standard ist das Dezimaltrennzeichen der aktuellen Region.

```csharp
public char NumberDecimalSeparator { get; set; }
```

### Beispiele

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

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


