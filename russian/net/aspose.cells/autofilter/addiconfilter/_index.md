---
title: "AutoFilter.AddIconFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Добавляет фильтр значков"
type: docs
url: /ru/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Добавляет фильтр по значку.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| iconSetType | IconSetType | Тип набора значков. |
| iconId | Int32 | Идентификатор значка. |

### Примечания

Поддерживает только добавление фильтра значков. Не поддерживает проверку, какая строка видима, если фильтр является фильтром значков.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить примерными данными столбец A
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // Получить экземпляр автофильтра
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Установить диапазон автофильтра (A1:A6) с использованием startRow, startColumn, endRow
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // Добавить фильтр значков в первый столбец (fieldIndex: 0)
                // Используется набор из 3 значков Traffic Lights (IconSetType.TrafficLights31)
                // Фильтрация по первому значку в наборе (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Обновить фильтр, чтобы применить изменения
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### См. также

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


