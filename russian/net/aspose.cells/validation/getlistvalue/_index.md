---
title: "Validation.GetListValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Получить значение списка проверки для указанной ячейки"
type: docs
url: /ru/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Получить значение списка проверок для указанной ячейки.

```csharp
public object GetListValue(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

Значение для формирования списка этой проверки для указанной ячейки. Если список ссылается на диапазон, то возвращаемое значение будет объектом [`ReferredArea`](../../referredarea/); в противном случае возвращаемое значение может быть null, object[] или простым объектом.

### Примечания

Только для проверки, тип которой List и которая применена к указанной ячейке; в остальных случаях будет возвращено null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для проверки
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // Создать проверку для ячейки B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // Тестировать GetListValue с различными параметрами
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // Изменить на значения, разделённые запятыми
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // Изменить на одно значение
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


