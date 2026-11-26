---
title: "IconSet.ShowValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство IconSet. Получить или установить флаг, указывающий, показывать ли значения ячеек, к которым применяется этот набор значков. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

Получить или установить флаг, указывающий, следует ли отображать значения ячеек, к которым применён этот набор значков. Значение по умолчанию — true.

```csharp
public bool ShowValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyShowValueDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);
            sheet.Cells["A5"].PutValue(50);

            // Добавить условное форматирование набора значков
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            int index = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[index];

            // Установить свойства набора значков
            condition.IconSet.Type = IconSetType.TrafficLights31;
            condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
            condition.IconSet.Reverse = false;

            // Установить диапазон для условного форматирования
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            formatConditions.AddArea(area);

            // Сохраните книгу
            workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
        }
    }
}
```

### См. также

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


