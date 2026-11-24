---
title: "ExportTableOptions.SkipErrorValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Eigenschaft. Gibt an, ob ungültige Werte für die Spalte übersprungen werden sollen. Zum Beispiel, wenn der Spaltentyp decimal ist und der Wert größer als decimal.MaxValue ist und diese Eigenschaft true ist, wird keine Ausnahme mehr ausgelöst. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

Gibt an, ob ungültige Werte für die Spalte übersprungen werden sollen. Zum Beispiel, wenn der Spaltentyp decimal ist, der Wert größer als decimal.MaxValue ist und diese Eigenschaft true ist, wird keine Ausnahme mehr ausgelöst. Der Standardwert ist false.

```csharp
public bool SkipErrorValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertySkipErrorValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;

            Worksheet ws = wb.Worksheets[0];

            // Erster Testfall – numerische Werte
            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
            Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56

            // Zweiter Testfall – gemischte Werte
            ws.Cells["A2"].Value = "dummy";
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"

            // Dritter Testfall – Export als Zeichenkette
            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


