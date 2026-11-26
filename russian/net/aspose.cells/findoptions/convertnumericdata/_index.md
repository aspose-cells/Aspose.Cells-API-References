---
title: "FindOptions.ConvertNumericData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Получает или задает значение, указывающее, следует ли преобразовывать найденное строковое значение в числовые данные"
type: docs
url: /ru/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Получает или задает значение, указывающее, следует ли преобразовывать значение искомой строки в числовые данные.

```csharp
public bool ConvertNumericData { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные, включая числовые значения в виде строк
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // Создайте параметры поиска и установите ConvertNumericData в true
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // Найдите значение даты (хранится как строка, но преобразуется в числовое во время поиска)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // Вывести результат.
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


