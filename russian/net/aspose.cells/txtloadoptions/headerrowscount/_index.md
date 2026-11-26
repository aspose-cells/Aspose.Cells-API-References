---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Количество строк заголовка, которое будет повторяться для расширенных листов"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

Количество строк заголовка, которые следует повторять для расширенных листов.

```csharp
public int HeaderRowsCount { get; set; }
```

### Примечания

Строки заголовка, указанные этим свойством, будут дублироваться для этих расширенных листов. Это свойство действует только когда [`ExtendToNextSheet`](../extendtonextsheet/) равно true.

### Примеры

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderRowsCountDemo
    {
        public static void Run()
        {
            // Создайте пример содержимого CSV
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // Создайте TxtLoadOptions с HeaderRowsCount, установленным в 1
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // Загрузите данные CSV в книгу
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Продемонстрируйте, что первая строка рассматривается как заголовок
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // Покажите строки данных (пропуская заголовок)
                Console.WriteLine("Data Rows:");
                for (int row = 1; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
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


