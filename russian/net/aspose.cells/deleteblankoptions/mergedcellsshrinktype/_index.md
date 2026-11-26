---
title: "DeleteBlankOptions.MergedCellsShrinkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteBlankOptions. Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов"
type: docs
url: /ru/net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Примечания

Для KeepHeaderOnly все ячейки в нём будут считаться пустыми, за исключением непустой ячейки в левом верхнем углу. Это значение свойства по умолчанию. Для None все ячейки в нём будут считаться непустыми. Для ShrinkToFit все ячейки за пределами области отображения содержимого будут считаться пустыми.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Настройте примерные данные с объединёнными ячейками
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");
            
            // Создайте параметры удаления с разными типами сжатия
            DeleteBlankOptions options = new DeleteBlankOptions();
            
            // Случай 1: KeepHeaderOnly
            options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Сбросить лист
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Случай 2: ShrinkToFit
            options.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After ShrinkToFit - Merged area adjusted: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Сбросить лист
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Случай 3: None
            options.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After None - Merged area unchanged: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
        }
    }
}
```

### См. также

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


