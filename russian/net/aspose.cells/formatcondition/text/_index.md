---
title: "FormatCondition.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Текстовое значение в условном правиле форматирования. Доступно только для типа containsText, notContainsText, beginsWith и endsWith. Значение по умолчанию — null."
type: docs
url: /ru/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

Текстовое значение в правиле условного форматирования "text contains". Действительно только для type = containsText, notContainsText, beginsWith и endsWith. Значение по умолчанию — null.

```csharp
public string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить условное форматирование
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // Добавить текстовое условие
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // Установите свойство text (демонстрируя русский текст)
            formatCondition.Text = "вс";

            // Применить стиль форматирования
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // Применить к ячейке A1
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // Сохранить и проверить
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


