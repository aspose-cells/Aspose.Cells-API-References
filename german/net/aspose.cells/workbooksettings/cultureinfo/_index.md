---
title: "WorkbookSettings.CultureInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Liest oder setzt die Systemkulturinfo"
type: docs
url: /de/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Liest oder setzt die Systemkulturinformationen.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Hinweise

Gibt null zurück, wenn die Kulturinfo nicht gesetzt ist und [`Region`](../region/) nicht gesetzt ist.

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            
            // Setzen Sie die Region auf Frankreich, um Änderungen der CultureInfo zu demonstrieren
            wb.Settings.Region = CountryCode.France;
            
            // Holen Sie das Gruppentrennzeichen aus der französischen Kultur
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // Erstellen Sie einen Stil mit benutzerdefiniertem Format und zeigen Sie das kulturangepasste Format
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // Demonstrieren Sie die Zahlenformatierung mit französischer Kultur
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells["A1"];
            cell.PutValue(123456.78);
            cell.SetStyle(style);
            style.Custom = "# ###,00 €";
            
            Console.WriteLine($"Formatted value: {cell.StringValue}");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


