---
title: "FormatCondition.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получает и задает тип условного формата"
type: docs
url: /ru/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Получает и задает, включен ли тип условного формата.

```csharp
public FormatConditionType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
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

            // Создайте условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Добавить условие форматирования с типом выражения (исправленные параметры)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // Установить стиль для условия
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Продемонстрировать использование свойства Type
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // Сохраните книгу
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


