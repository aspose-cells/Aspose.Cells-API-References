---
title: "Style.IsAlignmentApplied"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, следует ли применять форматирование выравнивания"
type: docs
url: /ru/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

Указывает, следует ли применять форматирование выравнивания.

```csharp
public bool IsAlignmentApplied { get; set; }
```

### Примечания

Только для именованного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsAlignmentAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            
            // Установить свойства выравнивания
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // Включить применение выравнивания
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // Проверить, что выравнивание применено
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


