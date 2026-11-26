---
title: "TxtSaveOptions.ExportQuotePrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Указывает, следует ли экспортировать знак одинарной кавычки как часть значения ячейки, когда для неё включён QuotePrefix. По умолчанию false"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/exportquoteprefix/
---
## TxtSaveOptions.ExportQuotePrefix property

Указывает, следует ли экспортировать знак одинарной кавычки как часть значения ячейки, когда для неё включён [`QuotePrefix`](../../style/quoteprefix/). По умолчанию false.

```csharp
public bool ExportQuotePrefix { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportQuotePrefixDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Добавьте примерные данные со специальными символами
            cells[0, 0].PutValue("a\\bcdef\"g");
            cells[0, 1].PutValue("f\"g");
            cells[0, 2].PutValue("a\\bcdg");
            cells[0, 3].PutValue("abcdefg");
            cells[0, 4].PutValue("efg");
            cells[0, 5].PutValue("'abc");

            // Создайте параметры сохранения TXT
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = ',',
                ExportQuotePrefix = true // Demonstrate ExportQuotePrefix property
            };

            // Сохранить с ExportQuotePrefix = true
            workbook.Save("output_with_exportquoteprefix.csv", saveOptions);

            // Измените разделитель и сохраните снова
            saveOptions.Separator = '\\';
            workbook.Save("output_with_backslash_separator.csv", saveOptions);

            Console.WriteLine("Files saved successfully with ExportQuotePrefix property.");
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


