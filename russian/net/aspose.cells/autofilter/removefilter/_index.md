---
title: "AutoFilter.RemoveFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Удаляет фильтр для столбца фильтра"
type: docs
url: /ru/net/aspose.cells/autofilter/removefilter/
---
## RemoveFilter(int, string) {#removefilter_1}

Удаляет фильтр для столбца фильтра.

```csharp
public void RemoveFilter(int fieldIndex, string criteria)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| критерий | String | Указанный критерий (строка; например, "101"). Он может быть только null или значением одной из ячеек в этом столбце. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodRemoveFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными для демонстрации
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["C2"].PutValue(999.99);
            
            worksheet.Cells["A3"].PutValue("Novel");
            worksheet.Cells["B3"].PutValue("Books");
            worksheet.Cells["C3"].PutValue(19.99);
            
            worksheet.Cells["A4"].PutValue("Smartphone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["C4"].PutValue(599.99);

            // Установить диапазон автофильтра (заголовки + 3 строки данных)
            worksheet.AutoFilter.SetRange(0, 0, 2);

            try
            {
                AutoFilter autoFilter = worksheet.AutoFilter;
                
                // Применить фильтр к столбцу Category (fieldIndex 1) для "Electronics"
                autoFilter.AddFilter(1, "Electronics");
                autoFilter.Refresh(); // Apply filter to hide non-matching rows
                
                // Удалить конкретный фильтр из столбца Category
                autoFilter.RemoveFilter(1, "Electronics");
                autoFilter.Refresh(); // Re-apply filter (now shows all rows)

                Console.WriteLine("RemoveFilter executed: Electronics filter removed from Category column.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("AutoFilterMethodRemoveFilterWithInt32StringDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveFilter(int) {#removefilter}

Удалить конкретный фильтр.

```csharp
public void RemoveFilter(int fieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Конкретный индекс фильтра |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveFilterWithInt32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Добавить фильтр
            filter.AddFilter(0, "Apple");
            filter.Refresh();
            
            Console.WriteLine("After adding filter - Visible rows:");
            PrintVisibleRows(worksheet);
            
            // Удалить фильтр
            filter.RemoveFilter(0);
            filter.Refresh();
            
            Console.WriteLine("\nAfter removing filter - Visible rows:");
            PrintVisibleRows(worksheet);
        }
        
        private static void PrintVisibleRows(Worksheet worksheet)
        {
            for (int i = 0; i < worksheet.Cells.MaxDataRow + 1; i++)
            {
                if (!worksheet.Cells.Rows[i].IsHidden)
                {
                    Console.WriteLine($"Row {i + 1}: {worksheet.Cells[i, 0].StringValue}");
                }
            }
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


