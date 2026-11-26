---
title: "Перечисление BackgroundType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.BackgroundType. Перечисляет типы шаблонов фона ячеек"
type: docs
url: /ru/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

Перечисляет типы шаблонов фона ячейки.

```csharp
public enum BackgroundType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Представляет диагональный штриховой узор. |
| DiagonalStripe | `8` | Представляет диагональный полосатый узор. |
| Gray6 | `18` | Представляет шаблон серого 6,25% |
| Gray12 | `17` | Представляет шаблон серого 12,5% |
| Gray25 | `4` | Представляет шаблон серого 25%. |
| Gray50 | `2` | Представляет шаблон серого 50%. |
| Gray75 | `3` | Представляет шаблон серого 75%. |
| HorizontalStripe | `5` | Представляет горизонтальный полосатый узор. |
| None | `0` | Представляет отсутствие фона. |
| ReverseDiagonalStripe | `7` | Представляет обратный диагональный полосатый узор. |
| Solid | `1` | Представляет сплошной узор. |
| ThickDiagonalCrosshatch | `10` | Представляет толстый диагональный штриховой узор. |
| ThinDiagonalCrosshatch | `16` | Представляет тонкий диагональный штриховой узор. |
| ThinDiagonalStripe | `14` | Представляет тонкий диагональный полосатый узор. |
| ThinHorizontalCrosshatch | `15` | Представляет тонкий горизонтальный штриховой узор. |
| ThinHorizontalStripe | `11` | Представляет тонкий горизонтальный полосатый узор. |
| ThinReverseDiagonalStripe | `13` | Представляет тонкий обратный диагональный полосатый узор. |
| ThinVerticalStripe | `12` | Представляет тонкий вертикальный полосатый узор. |
| VerticalStripe | `6` | Представляет вертикальный полосатый узор. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к ячейке листа
            Cell cell = worksheet.Cells["A1"];
            
            // Установить значение ячейки
            cell.PutValue("Hello, Aspose!");

            // Создать объект стиля
            Style style = cell.GetStyle();
            
            // Установить тип фонового узора
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // Установить цвет переднего плана
            style.ForegroundColor = Color.Red;
            
            // Установить цвет фона
            style.BackgroundColor = Color.Green;
            
            // Применить стиль к ячейке
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


