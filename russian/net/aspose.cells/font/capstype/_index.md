---
title: "Font.CapsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает и задает тип заглавных букв текста"
type: docs
url: /ru/net/aspose.cells/font/capstype/
---
## Font.CapsType property

Получает и задает тип заглавных букв текста.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### Примечания

Только для шрифтов фигур или диаграмм. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCapsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("sample text");

            Style style = cell.GetStyle();
            style.Font.CapsType = TextCapsType.All;
            cell.SetStyle(style);

            workbook.Save("FontCapsTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


