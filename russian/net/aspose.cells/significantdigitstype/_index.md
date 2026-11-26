---
title: "Перечисление SignificantDigitsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.SignificantDigitsType. Представляет тип значимых цифр для вывода числовых значений"
type: docs
url: /ru/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Представляет тип значимых цифр при выводе числовых значений.

```csharp
public enum SignificantDigitsType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Digits15 | `0` | 15-цифр |
| G17 | `1` | 17-цифр путем форматирования значения с помощью "G17". |
| Rounding17 | `2` | 17-цифр путем округления значения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу для демонстрации
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Продемонстрировать использование каждого значения перечисления SignificantDigitsType
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Установите тип значимых цифр для рабочей книги
                    workbook.Settings.SignificantDigitsType = type;

                    // Отобразите текущую настройку
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Добавьте пример значения, чтобы продемонстрировать настройку
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Сохраните рабочую книгу с текущей настройкой
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


