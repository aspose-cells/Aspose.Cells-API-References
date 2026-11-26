---
title: "IconFilter.IconSetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство IconFilter. Получает и задает набор значков, используемый для этих критериев фильтра"
type: docs
url: /ru/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Получает и задает набор значков, используемый для этого критерия фильтра.

```csharp
public IconSetType IconSetType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Создать автофильтр
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Получить фильтр значков
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Отобразить текущий IconSetType (по умолчанию None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // Установить набор значков из 3 стрелок
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Применить условное форматирование для визуализации значков
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Переключить на набор значков светофоров
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Сохранить результат
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


