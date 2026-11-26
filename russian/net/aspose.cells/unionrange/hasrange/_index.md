---
title: "UnionRange.HasRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Указывает, содержит ли он диапазон"
type: docs
url: /ru/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Указывает, имеет ли это диапазон.

```csharp
public bool HasRange { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyHasRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте объединённый диапазон, используя правильный API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Проверьте, имеет ли объединённый диапазон действительные диапазоны
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // Установите значение и стиль только если диапазон действителен
            if (unionRange.HasRange)
            {
                unionRange.Value = "Test Value";
                
                Style style = workbook.CreateStyle();
                style.Pattern = BackgroundType.Solid;
                style.ForegroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });
            }
            
            workbook.Save("UnionRangeHasRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


