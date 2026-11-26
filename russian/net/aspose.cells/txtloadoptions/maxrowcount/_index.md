---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Максимальное количество строк, импортируемых в один лист"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

Максимальное количество строк, импортируемых в один лист.

```csharp
public int MaxRowCount { get; set; }
```

### Примечания

Строки, превышающие этот предел, будут игнорироваться или переноситься на следующий лист в соответствии с [`ExtendToNextSheet`](../extendtonextsheet/). Это количество включает строки заголовка ([`HeaderRowsCount`](../headerrowscount/)). Максимально допустимое значение равно ограничению количества строк соответствующего формата файла, например для файла xlsx это 1048576. Если это свойство не указано или указанное значение не положительно, будет использовано максимальное ограничение.

### Примеры

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // Создайте пример содержимого CSV
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // Создать TxtLoadOptions с MaxRowCount, установленным в 4
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // Загрузить CSV в рабочую книгу
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // Проверьте, что загружено только 4 строки (1 заголовок + 3 строки данных)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // Это будет null, поскольку мы загрузили только 4 строки (индексы 0‑3)
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
                }
            }
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


