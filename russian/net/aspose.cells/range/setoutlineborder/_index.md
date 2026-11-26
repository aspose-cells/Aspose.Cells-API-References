---
title: "Range.SetOutlineBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Устанавливает контурную границу вокруг диапазона ячеек"
type: docs
url: /ru/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Устанавливает контурную границу вокруг диапазона ячеек.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderEdge | BorderType | Край границы. |
| borderStyle | CellBorderType | Стиль границы. |
| borderColor | CellsColor | Цвет границы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте объект CellsColor
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Создайте диапазон и установите правую границу
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // Создайте другой диапазон и установите все границы
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Сохраните книгу
            workbook.Save("SetOutlineBorderExample.xlsx");
        }
    }
}
```

### См. также

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Устанавливает контурную границу вокруг диапазона ячеек.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderEdge | BorderType | Край границы. |
| borderStyle | CellBorderType | Стиль границы. |
| borderColor | Color | Цвет границы. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон ячеек
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // Установите контурные границы с разными типами границ и цветами
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // Сохраните книгу
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### См. также

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


