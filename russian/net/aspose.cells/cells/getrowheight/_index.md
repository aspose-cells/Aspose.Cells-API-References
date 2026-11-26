---
title: "Cells.GetRowHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает высоту строк"
type: docs
url: /ru/net/aspose.cells/cells/getrowheight/
---
## GetRowHeight(int, bool, CellsUnitType) {#getrowheight_1}

Получает высоту строки.

```csharp
public double GetRowHeight(int row, bool isOriginal, CellsUnitType unitType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| isOriginal | Boolean | Возвращает ли оригинальную высоту строки или 0 для скрытой строки. |
| unitType | CellsUnitType | Тип единицы измерения возвращаемого значения высоты |

### Возвращаемое значение

Высота строки

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить высоту строки для строки 3 (20 пикселей)
            worksheet.Cells.SetRowHeightPixel(3, 20);
            
            // Получить высоту строки в разных единицах измерения
            double heightInPixels = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Pixel);
            double heightInPoints = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Point);
            
            // Выведите результаты
            Console.WriteLine("Row height in pixels: " + heightInPixels);
            Console.WriteLine("Row height in points: " + heightInPoints);
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

## GetRowHeight(int) {#getrowheight}

Получает высоту указанной строки в пунктах.

```csharp
public double GetRowHeight(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |

### Возвращаемое значение

Высота строки

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets["Sheet1"];
            Cells cells = ws.Cells;
            
            string strText = "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.";
            cells[0, 0].PutValue(strText);
            
            Style style = cells[0, 0].GetStyle();
            style.IsTextWrapped = true;
            cells[0, 0].SetStyle(style);
            
            ws.Cells.SetColumnWidth(0, 50);
            ws.AutoFitRows();
            
            double rowHeight = cells.GetRowHeight(0);
            Console.WriteLine("Row height: " + rowHeight);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


