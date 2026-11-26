---
title: "Перечисление CellBorderType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.CellBorderType перечисление. Перечисляет тип границы ячейки."
type: docs
url: /ru/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

Перечисляет тип границы ячейки.

```csharp
public enum CellBorderType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DashDot | `9` | Представляет тонкую пунктирно‑штриховую линию. |
| DashDotDot | `11` | Представляет тонкую пунктирно‑точечную линию. |
| Dashed | `3` | Представляет пунктирную линию. |
| Dotted | `4` | Представляет пунктирную линию. |
| Double | `6` | Представляет двойную линию. |
| Hair | `7` | Представляет тонкую линию. |
| MediumDashDot | `10` | Представляет среднюю пунктирно‑штриховую линию. |
| MediumDashDotDot | `12` | Представляет среднюю пунктирно‑точечную линию. |
| MediumDashed | `8` | Представляет среднюю пунктирную линию. |
| None | `0` | Не представляет линию. |
| Medium | `2` | Представляет среднюю линию. |
| SlantedDashDot | `13` | Представляет наклонную среднюю пунктирно‑штриховую линию. |
| Thick | `5` | Представляет толстую линию. |
| Thin | `1` | Представляет тонкую линию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Получить стиль диапазона
            Style style = workbook.CreateStyle();

            // Установить различные стили границ для диапазона
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // Применить стиль к диапазону
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // Сохраните книгу
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


