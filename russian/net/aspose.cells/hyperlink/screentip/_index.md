---
title: "Hyperlink.ScreenTip"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Hyperlink. Возвращает или задает текст ScreenTip для указанной гиперссылки"
type: docs
url: /ru/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Возвращает или задает текст ScreenTip для указанной гиперссылки.

```csharp
public string ScreenTip { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // Создайте гиперссылку с ScreenTip
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // Сохраните книгу
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### См. также

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


