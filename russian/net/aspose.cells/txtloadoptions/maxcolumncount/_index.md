---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Максимальное количество столбцов, импортируемых в один лист"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

Максимальное количество столбцов, импортируемых в один лист.

```csharp
public int MaxColumnCount { get; set; }
```

### Примечания

Столбцы, превышающие этот предел, будут игнорироваться или переноситься на следующий лист в соответствии с [`ExtendToNextSheet`](../extendtonextsheet/). Это количество включает столбцы заголовка ([`HeaderColumnsCount`](../headercolumnscount/)). Максимальное значение равно ограничению количества столбцов соответствующего формата файла, например для файла xlsx это 16384. Если это свойство не указано или указанное значение не положительно, будет использовано максимальное ограничение.

### Примеры

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxColumnCountDemo
    {
        public static void Run()
        {
            // Создайте пример содержимого CSV
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // Создать TxtLoadOptions с MaxColumnCount, установленным в 5
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // Загрузить CSV с ограниченными столбцами
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Вывести загруженные данные (должны присутствовать только первые 5 столбцов)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Проверьте, что загружено только 5 столбцов
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


