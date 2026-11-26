---
title: "Range.AddHyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Добавляет гиперссылку в указанную ячейку или диапазон ячеек."
type: docs
url: /ru/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| address | String | Адрес гиперссылки. |
| textToDisplay | String | Текст, который будет отображаться для указанной гиперссылки. |
| screenTip | String | Текст screenTip для указанной гиперссылки. |

### Возвращаемое значение

[`Hyperlink`](../../hyperlink/) object.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // Добавить гиперссылку с адресом, отображаемым текстом и подсказкой.
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // Сохраните книгу
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### См. также

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


