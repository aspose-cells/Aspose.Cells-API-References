---
title: "ExportTableOptions.SkipErrorValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportTableOptions. Indica se ignorare i valori non validi per la colonna. Per esempio, se il tipo della colonna è decimal e il valore è maggiore di decimal.MaxValue e questa proprietà è true, non verrà sollevata nuovamente un'eccezione. Il valore predefinito è false."
type: docs
url: /it/net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

Indica se ignorare i valori non validi per la colonna. Ad esempio, se il tipo della colonna è decimal, il valore è maggiore di decimal.MaxValue e questa proprietà è true, non verrà sollevata nuovamente un'eccezione. Il valore predefinito è false.

```csharp
public bool SkipErrorValue { get; set; }
```

### Esempi

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

            // Primo caso di test - valori numerici
            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
            Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56

            // Secondo caso di test - valori misti
            ws.Cells["A2"].Value = "dummy";
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"

            // Terzo caso di test - esporta come stringa
            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


