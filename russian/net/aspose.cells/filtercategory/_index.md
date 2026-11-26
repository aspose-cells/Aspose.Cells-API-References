---
title: "Перечисление FilterCategory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FilterCategory. Представляет категорию фильтра"
type: docs
url: /ru/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

Представляет категорию фильтра.

```csharp
public enum FilterCategory
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без фильтра. |
| Label | `1` | Фильтр подписи. |
| NumberValue | `2` | Фильтр числового значения. |
| Date | `3` | Фильтр даты. |
| Top10 | `4` | Фильтр Top10 значений. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            CreateSampleData(worksheet);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Настроить поля строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // Настроить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Добавить фильтр метки к фильтрам сводной таблицы
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // Продемонстрировать использование FilterCategory
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // Отобразить все категории фильтров в сводной таблице
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохранить результат
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Установить заголовки примерных данных
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // Добавить строки примерных данных
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


