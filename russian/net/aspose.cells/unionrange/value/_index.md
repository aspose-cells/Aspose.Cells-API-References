---
title: "UnionRange.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Получает и задает значения диапазона"
type: docs
url: /ru/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Получает и задаёт значения диапазона.

```csharp
public object Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте объединённый диапазон, используя правильный API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // Установить значение для всего объединённого диапазона
            unionRange.Value = "Test Value";
            
            // Создайте и примените стиль
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Сохраните книгу
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


