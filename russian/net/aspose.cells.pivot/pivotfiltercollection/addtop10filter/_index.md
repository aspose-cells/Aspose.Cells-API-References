---
title: "PivotFilterCollection.AddTop10Filter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilterCollection. Фильтрует по значениям поля сводных данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfiltercollection/addtop10filter/
---
## PivotFilterCollection.AddTop10Filter method

Фильтрует по значениям данных сводного поля.

```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    bool isTop, int itemCount)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | Int32 | Индекс поля в источнике. |
| valueFieldIndex | Int32 | Индекс поля данных в области данных. |
| type | PivotFilterType | Тип фильтрации данных. Может быть только Count, Sum и Percent. |
| isTop | Boolean | Указывает, применяется ли фильтр сверху или снизу |
| itemCount | Int32 | Количество элементов |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Dairy";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 80;
            worksheet.Cells["B4"].Value = 120;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Получить коллекцию сводных фильтров
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Добавить фильтр Top10 — показать 2 лучших элемента по продажам
                PivotFilter filter = filters.AddTop10Filter(
                    baseFieldIndex: 0,          // Category field
                    valueFieldIndex: 1,          // Sales field
                    type: PivotFilterType.Count, // Filter type
                    isTop: true,                 // Show top items
                    itemCount: 2                 // Number of items to show
                );

                Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


