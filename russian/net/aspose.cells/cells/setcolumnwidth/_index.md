---
title: "Cells.SetColumnWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Устанавливает ширину указанного столбца в обычном виде"
type: docs
url: /ru/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Устанавливает ширину указанного столбца в обычном виде.

```csharp
public void SetColumnWidth(int column, double width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| ширина | Double | Ширина столбца в единицах символов. Ширина столбца должна быть от 0 до 255. |

### Примечания

Для электронных таблиц ширина столбца измеряется количеством символов максимальной ширины цифр чисел 0~9, отображаемых шрифтом обычного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


