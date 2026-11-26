---
title: "FontSettingCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSettingCollection. Получает FontSetting по индексу"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

Получает [`FontSetting`](../../../aspose.cells/fontsetting/) по индексу.

```csharp
public FontSetting this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook w = new Workbook();
            Worksheet s = w.Worksheets[0];

            Shape tb = s.Shapes.AddTextBox(3, 0, 7, 0, 70, 300);
            tb.Text = "Sample Text";

            // Установить свойства шрифта для конкретных символов
            Aspose.Cells.Font fo = tb.Characters(3, 5).Font;
            fo.IsSuperscript = true;
            fo.Color = Color.Red;

            // Получить шрифт через свойство TextBody.Item
            Aspose.Cells.Font fo1 = tb.TextBody[3].Font;
            Console.WriteLine("IsSuperscript: " + fo1.IsSuperscript);
            Console.WriteLine("Color: " + fo1.Color);

            w.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


