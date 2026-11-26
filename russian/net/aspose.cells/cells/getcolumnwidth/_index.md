---
title: "Cells.GetColumnWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Cells method. Получает ширину столбца"
type: docs
url: /ru/net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

Получает ширину столбца.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| isOriginal | Boolean | Указывает, получаем ли оригинальную ширину. |
| unitType | CellsUnitType |  |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить ширину столбца для столбца 1 (индекс с нуля)
            cells.SetColumnWidth(0, 20);

            // Получить ширину столбца в разных единицах и режимах
            double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
            double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
            double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);

            Console.WriteLine("Column width in pixels: " + widthInPixels);
            Console.WriteLine("Column width in points: " + widthInPoints);
            Console.WriteLine("Default column width: " + defaultWidth);
        }
    }
}
```

### См. также

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidth(int) {#getcolumnwidth}

Получает ширину (в единицах символов) указанного столбца в обычном виде.

```csharp
public double GetColumnWidth(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца |

### Возвращаемое значение

Ширина столбца. Для электронных таблиц ширина столбца измеряется количеством символов максимальной ширины цифры чисел 0~9, отображаемых шрифтом обычного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить ширину столбца для индекса столбца 255
            cells.SetColumnWidth(255, 20.86);

            // Получить и отобразить ширину столбца
            double columnWidth = cells.GetColumnWidth(255);
            Console.WriteLine("Column width at index 255: " + columnWidth);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


