---
title: "TxtLoadOptions.HeaderColumnsCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Количество столбцов заголовка, которые будут повторяться для расширенных листов"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

Количество столбцов заголовка, которые следует повторять для расширенных листов.

```csharp
public int HeaderColumnsCount { get; set; }
```

### Примечания

Столбцы заголовка, указанные этим свойством, будут дублироваться для этих расширенных листов. Это свойство действует только когда [`ExtendToNextSheet`](../extendtonextsheet/) равно true.

### Примеры

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderColumnsCountDemo
    {
        public static void Run()
        {
            // Создайте пример содержимого CSV
            string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
                            "H1,H2,H3,D1,D2,D3\n" +
                            "A,B,C,D,E,F\n" +
                            "G,H,I,J,K,L";

            // Создать TxtLoadOptions с HeaderColumnsCount, установленным в 3
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderColumnsCount = 3, // First 3 columns will be treated as headers
                Encoding = Encoding.UTF8
            };

            // Загрузите данные CSV в книгу
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Продемонстрировать столбцы заголовка (первые 3 столбца)
                Console.WriteLine("Header Columns:");
                for (int row = 0; row < 2; row++)
                {
                    for (int col = 0; col < options.HeaderColumnsCount; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Продемонстрировать столбцы данных (оставшиеся столбцы)
                Console.WriteLine("\nData Columns:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = options.HeaderColumnsCount; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
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


