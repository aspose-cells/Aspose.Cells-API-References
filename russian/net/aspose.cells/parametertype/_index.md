---
title: "Перечисление ParameterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ParameterType. Представляет типы всех параметров или тип возвращаемого значения функции"
type: docs
url: /ru/net/aspose.cells/parametertype/
---
## ParameterType enumeration

Представляет тип всех параметров или тип возвращаемого значения функции.

```csharp
public enum ParameterType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // Создание рабочей книги и листа для демонстрации использования
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример использования перечисления ParameterType в формульной функции
            // Предположим, что мы определяем пользовательскую функцию с конкретными типами параметров

            // Определить массив типов параметров
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // Пример функции, использующей эти типы параметров
            // Например, настройка гипотетической пользовательской функции с определёнными типами параметров
            // (Примечание: Обработка пользовательских функций будет зависеть от возможностей API Aspose.Cells)

            // Сохранить рабочую книгу, чтобы продемонстрировать изменения
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


