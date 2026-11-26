---
title: "Slicer.LockedPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Slicer property. Указывает, может ли указанный срез перемещаться или изменять размер с помощью пользовательского интерфейса"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

Указывает, можно ли перемещать или изменять размер указанного slicer с помощью пользовательского интерфейса.

```csharp
public bool LockedPosition { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Создать коллекцию сводных таблиц
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Создайте сводную таблицу
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Создать коллекцию срезов
            SlicerCollection slicers = worksheet.Slicers;
            
            // Добавить срез для сводной таблицы
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // Установить свойства слайсера
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // Продемонстрировать свойство LockedPosition
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Изменить LockedPosition на false, чтобы разрешить перемещение
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Сохраните книгу
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


