---
title: "ConditionalFormattingIcon.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingIcon. Получает и задает тип набора значков"
type: docs
url: /ru/net/aspose.cells/conditionalformattingicon/type/
---
## ConditionalFormattingIcon.Type property

Получает и устанавливает тип набора значков.

```csharp
public IconSetType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Добавить условное форматирование с набором иконок
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fc = cfs[index];
            fc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            int conditionIndex = fc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fc[conditionIndex];
            condition.IconSet.Type = IconSetType.Symbols3;
            
            // Примените форматирование и выполните расчёт
            workbook.CalculateFormula();

            // Получите результат форматирования и продемонстрируйте свойство Type
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("Icon Set Type: " + formattingResult.ConditionalFormattingIcon.Type);
            Console.WriteLine("Icon Index: " + formattingResult.ConditionalFormattingIcon.Index);
        }
    }
}
```

### См. также

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


