---
title: "Range.SetOutlineBorders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы"
type: docs
url: /ru/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | CellBorderType | Стиль границы. |
| borderColor | CellsColor | Цвет границы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBordersWithCellBorderTypeCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать объект CellsColor с цветом темы
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Создать диапазон и установить контурные границы
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Сохраните книгу
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyle | CellBorderType | Стиль границы. |
| borderColor | Color | Цвет границы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон ячеек (A1:D4)
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Заполнить диапазон данными, чтобы границы были видимы
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // Вызвать SetOutlineBorders со средним стилем границы и красным цветом
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // Сохранить рабочую книгу, чтобы увидеть эффект
                workbook.Save("RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Устанавливает внешние границы вокруг диапазона ячеек.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Стили границ. |
| borderColors | Color[] | Цвета границ. |

### Примечания

Длина массивов borderStyles и borderStyles должна быть 4. Порядок элементов в borderStyles и borderStyles должен быть верх,низ,лево,право

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон ячеек (B2:D4)
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // Подготовить стили границ и цвета
            CellBorderType[] borderStyles = new CellBorderType[]
            {
                CellBorderType.Thick,
                CellBorderType.Dashed,
                CellBorderType.Double,
                CellBorderType.MediumDashDot
            };

            Color[] borderColors = new Color[]
            {
                Color.Red,
                Color.Blue,
                Color.Green,
                Color.Purple
            };

            try
            {
                // Установить контурные границы с разными стилями и цветами
                range.SetOutlineBorders(borderStyles, borderColors);

                // Заполнить ячейки данными, чтобы границы были видимы
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // Сохраните книгу
                workbook.Save("RangeSetOutlineBordersDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


