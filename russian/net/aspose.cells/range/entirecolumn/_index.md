---
title: "Range.EntireColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает объект Range, который представляет всю колонку или колонки, содержащие указанный диапазон"
type: docs
url: /ru/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон.

```csharp
public Range EntireColumn { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте диапазон, начинающийся с ячейки C1 (строка 0, столбец 2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // Получите всю колонку, содержащую диапазон (колонка C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // Примените форматирование ко всей колонке
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // Сохраните книгу
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


