---
title: "PivotFilterCollection.AddDateFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilterCollection. Фильтрует по настройкам даты строкового или столбцового сводного поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfiltercollection/adddatefilter/
---
## PivotFilterCollection.AddDateFilter method

Фильтрует по настройке даты строки или столбца сводного поля.

```csharp
public PivotFilter AddDateFilter(int baseFieldIndex, PivotFilterType type, DateTime dateTime1, 
    DateTime dateTime2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | Int32 | Индекс поля в источнике. |
| type | PivotFilterType | Тип данных фильтрации. |
| dateTime1 | DateTime | Метка даты условия фильтра |
| dateTime2 | DateTime | Верхняя метка даты условия фильтра «между» |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddDateFilterWithInt32PivotFilterTypeDateTimeDaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные с датами
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Добавить фильтр даты, чтобы показывать даты между 1 января и 31 марта 2023 г.
                PivotFilter filter = filters.AddDateFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.DateBetween,
                    dateTime1: new DateTime(2023, 1, 1),
                    dateTime2: new DateTime(2023, 3, 31)
                );

                Console.WriteLine($"Date filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, UseWholeDay: {filter.UseWholeDay}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding date filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddDateFilterDemo.xlsx");
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


