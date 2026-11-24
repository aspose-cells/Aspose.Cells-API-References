---
title: "WorkbookSettings.NumberGroupSeparator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt das Zeichen zurück oder legt es fest, das Gruppen von Ziffern links vom Dezimaltrennzeichen in numerischen Werten trennt. Der Standard ist das Gruppentrennzeichen der aktuellen Region."
type: docs
url: /de/net/aspose.cells/workbooksettings/numbergroupseparator/
---
## WorkbookSettings.NumberGroupSeparator property

Liest oder setzt das Zeichen, das Gruppen von Ziffern links vom Dezimaltrennzeichen in numerischen Werten trennt. Standard ist das Gruppentrennzeichen der aktuellen Region.

```csharp
public char NumberGroupSeparator { get; set; }
```

### Beispiele

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

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


