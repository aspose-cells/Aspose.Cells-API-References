---
title: "Range.SetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Применить стиль ячейки"
type: docs
url: /ru/net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Применить стиль ячейки.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Стиль ячейки. |
| explicitFlag | Boolean | True, только перезаписывая форматирование, которое явно задано. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
            range.SetStyle(style, true);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Устанавливает стиль диапазона.

```csharp
public void SetStyle(Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Объект Style. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать стиль
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.Font.Color = Color.Red;
            style.Font.Underline = FontUnderlineType.Single;

            // Применить стиль к ячейке
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].SetStyle(style);

            // Создайте диапазон и примените тот же стиль
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
            range.SetStyle(style);

            // Сохраните книгу
            workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


