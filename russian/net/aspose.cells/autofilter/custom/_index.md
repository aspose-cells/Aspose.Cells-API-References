---
title: "AutoFilter.Custom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Фильтрует список с пользовательским критерием."
type: docs
url: /ru/net/aspose.cells/autofilter/custom/
---
## Custom(int, FilterOperatorType, object) {#custom}

Фильтрует список с пользовательским критерием.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| operatorType1 | FilterOperatorType | Тип оператора фильтра |
| criteria1 | Object | Пользовательский критерий |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в столбец A (10 строк + заголовок)
            worksheet.Cells["A1"].PutValue("Numbers");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i); // A2-A11: 1-10
            }

            // Установить диапазон autofilter (A1:A11)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Применить пользовательский фильтр: Числа > 5
                worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterThan, 5);
                
                // Обновить фильтр, чтобы применить изменения
                worksheet.AutoFilter.Refresh();
                
                Console.WriteLine("Custom filter applied: Column 0 values > 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }
            
            // Сохранить отфильтрованную рабочую книгу
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Custom(int, FilterOperatorType, object, bool, FilterOperatorType, object) {#custom_1}

Фильтрует список с пользовательскими критериями.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1, bool isAnd, 
    FilterOperatorType operatorType2, object criteria2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| operatorType1 | FilterOperatorType | Тип оператора фильтра |
| criteria1 | Object | Пользовательский критерий |
| isAnd | Boolean |  |
| operatorType2 | FilterOperatorType | Тип оператора фильтра |
| criteria2 | Object | Пользовательский критерий |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными
            worksheet.Cells["A1"].PutValue("Product ID");
            worksheet.Cells["A2"].PutValue(85);
            worksheet.Cells["A3"].PutValue(42);
            worksheet.Cells["A4"].PutValue(65);
            worksheet.Cells["A5"].PutValue(95);
            worksheet.Cells["A6"].PutValue(30);
            worksheet.Cells["A7"].PutValue(75);

            // Установить диапазон auto filter (A1:A7)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 0); // Start row: 0 (A1), strartt column: 0 (A), end Column: 0 (A)

            try
            {
                // Применить пользовательский фильтр: больше или равно 50 И меньше или равно 100
                autoFilter.Custom(
                    0, // Field index (column A)
                    FilterOperatorType.GreaterOrEqual,
                    50, // First criteria
                    true, // AND combination
                    FilterOperatorType.LessOrEqual,
                    100 // Second criteria
                );

                Console.WriteLine("Custom filter applied successfully with parameters: " +
                    "(Int32, FilterOperatorType, Object, Boolean, FilterOperatorType, Object)");

                // Обновить фильтры и сохранить результаты
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }

            // Сохранить отфильтрованную рабочую книгу
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


