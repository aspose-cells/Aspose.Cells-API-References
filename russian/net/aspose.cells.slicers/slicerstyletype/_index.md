---
title: "Перечисление SlicerStyleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Slicers.SlicerStyleType. Укажите стиль отображения слайсера"
type: docs
url: /ru/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Укажите стиль представления среза

```csharp
public enum SlicerStyleType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | встроенный светлый стиль один |
| SlicerStyleLight2 | `1` | встроенный светлый стиль два |
| SlicerStyleLight3 | `2` | встроенный светлый стиль три |
| SlicerStyleLight4 | `3` | встроенный светлый стиль четыре |
| SlicerStyleLight5 | `4` | встроенный светлый стиль пять |
| SlicerStyleLight6 | `5` | встроенный светлый стиль шесть |
| SlicerStyleOther1 | `6` | встроенный стиль другой один |
| SlicerStyleOther2 | `7` | встроенный стиль другой два |
| SlicerStyleDark1 | `8` | встроенный тёмный стиль один |
| SlicerStyleDark2 | `9` | встроенный тёмный стиль два |
| SlicerStyleDark3 | `10` | встроенный тёмный стиль три |
| SlicerStyleDark4 | `11` | встроенный тёмный стиль четыре |
| SlicerStyleDark5 | `12` | встроенный тёмный стиль пять |
| SlicerStyleDark6 | `13` | встроенный тёмный стиль шесть |
| Custom | `14` | пользовательский стиль, пока не поддерживается |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить срез
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Установить стиль среза
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // Сохраните книгу
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


