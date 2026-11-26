---
title: "IconFilter.IconId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство IconFilter. Получает и задает нулевой индекс значка в наборе значков"
type: docs
url: /ru/net/aspose.cells/iconfilter/iconid/
---
## IconFilter.IconId property

Получает и задает нулевой индекс значка в наборе значков.

```csharp
public int IconId { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Применить условное форматирование набора значков
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.TrafficLights31;
            
            // Установить диапазон с помощью CellArea
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Создать автофильтр с фильтром значков
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;
            
            // Получить существующий фильтр вместо создания нового экземпляра
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 0;

            Console.WriteLine("Current IconId value: " + iconFilter.IconId);

            // Изменить IconId для фильтрации разных значков
            iconFilter.IconId = 1;

            workbook.Save("PropertyIconIdDemo.xlsx");
        }
    }
}
```

### См. также

* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


