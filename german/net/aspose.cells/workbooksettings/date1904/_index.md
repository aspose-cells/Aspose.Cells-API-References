---
title: "WorkbookSettings.Date1904"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings‑Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Arbeitsmappe das 1904‑Datumssystem verwendet"
type: docs
url: /de/net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Liest oder setzt einen Wert, der angibt, ob das Workbook das 1904-Datumsystem verwendet.

```csharp
public bool Date1904 { get; set; }
```

### Beispiele

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
            
            // Demonstriere negative Zeit mit Date1904
            Style style = cell.GetStyle();
            style.Custom = "h:mm";
            cell.SetStyle(style);
            cell.PutValue(-0.0736111111111112);
            Console.WriteLine("Negative time value: " + cell.DisplayStringValue);

            // Demonstriere negatives Datum mit Date1904
            style = cell.GetStyle();
            style.Custom = "mm/dd/yyyy h:mm:ss";
            cell.SetStyle(style);
            cell.PutValue(-42389.47075706);
            Console.WriteLine("Negative date value: " + cell.DisplayStringValue);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


