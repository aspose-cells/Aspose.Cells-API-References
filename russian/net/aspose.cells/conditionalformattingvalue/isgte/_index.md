---
title: "ConditionalFormattingValue.IsGTE"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingValue. Получить или установить флаг «Больше или равно». Используется только для наборов значков, определяет, использует ли это пороговое значение оператор «больше или равно». false указывает, что используется «больше», а не «больше или равно». Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Получить или установить флаг Greater Than Or Equal. Используется только для наборов значков, определяет, использует ли это пороговое значение оператор «больше или равно». Значение 'false' указывает, что используется «больше», а не «больше или равно». Значение по умолчанию — true.

```csharp
public bool IsGTE { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Добавьте примерные данные
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // Добавить условное форматирование
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // Создать формат цветовой шкалы
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // Настроить шкалу из 2 цветов
            fc.ColorScale.Is3ColorScale = false;
            
            // Установить формат максимального значения (демонстрация IsGTE)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // Установить формат минимального значения
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // Сохраните книгу
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


