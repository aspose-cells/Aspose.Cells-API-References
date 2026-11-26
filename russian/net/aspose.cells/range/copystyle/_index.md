---
title: "Range.CopyStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Копирует настройки стиля из исходного диапазона"
type: docs
url: /ru/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Копирует настройки стиля из исходного диапазона.

```csharp
public void CopyStyle(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| range | Range | Исходный объект [`Range`](../). |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // Добавьте примерный стиль в исходный диапазон
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // Создать лист назначения
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // Создать диапазон назначения и скопировать стиль
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // Сохраните книгу
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


