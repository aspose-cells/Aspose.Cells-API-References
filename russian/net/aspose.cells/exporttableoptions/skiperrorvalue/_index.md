---
title: "ExportTableOptions.SkipErrorValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Указывает, следует ли пропускать недопустимое значение для столбца. Например, если тип столбца — decimal и значение превышает decimal.MaxValue, и это свойство равно true, исключение выбрасываться не будет. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

Указывает, следует ли пропускать недопустимые значения для столбца. Например, если тип столбца decimal, значение превышает decimal.MaxValue и это свойство равно true, исключение выброшено не будет. Значение по умолчанию — false.

```csharp
public bool SkipErrorValue { get; set; }
```

### Примеры

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

            // Первый тестовый случай — числовые значения
            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
            Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56

            // Второй тестовый случай — смешанные значения
            ws.Cells["A2"].Value = "dummy";
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"

            // Третий тестовый случай — экспорт как строка
            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


