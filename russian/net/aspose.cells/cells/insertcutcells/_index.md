---
title: "Cells.InsertCutCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Вставить вырезанный диапазон"
type: docs
url: /ru/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Вставить вырезанный диапазон.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cutRange | Диапазон | Вырезаемый диапазон. |
| строка | Int32 | Строка. |
| column | Int32 | Столбец. |
| shiftType | ShiftType | Указывает, как смещать другие объекты целевого диапазона при вставке вырезаемого диапазона. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу и его ячейкам
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // Добавьте некоторые данные в исходные ячейки
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // Создайте второй лист как назначение
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // Добавьте некоторые начальные данные в назначение
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // Создайте диапазон для вырезания (A1:B2 из исходного листа)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // Вставьте вырезанные ячейки в B2 на листе назначения, сместив ячейки вниз
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // Сохраните книгу
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


