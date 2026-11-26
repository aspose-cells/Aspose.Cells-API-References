---
title: "Validation.GetValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Получить значение проверки в конкретной ячейке"
type: docs
url: /ru/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Получить значение проверки в конкретной ячейке.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |
| isValue1 | Boolean | Указывает, получено ли первое значение. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные и проверку
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // Создать проверку для ячейки B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // Получить значение с помощью метода GetValue, указав параметры строки, столбца и преобразования числового значения в дату
            object value = validation.GetValue(0, 1, false);
            
            // Вывести результат.
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


