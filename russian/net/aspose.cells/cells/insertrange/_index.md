---
title: "Cells.InsertRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Вставляет диапазон ячеек и сдвигает ячейки в соответствии с параметром сдвига"
type: docs
url: /ru/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| область | CellArea | Сместить область. |
| shiftNumber | Int32 | Количество строк или столбцов для вставки. |
| shiftType | ShiftType | Опция смещения ячеек. |
| updateReference | Boolean | Указывает, следует ли обновлять ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните некоторыми образцовыми данными
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // Определите область для вставки (строки 2‑3, столбец A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // Вставить диапазон, сместив ячейки вправо, и обновить ссылки
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // Проверьте операцию, проверив значения
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| область | CellArea | Сместить область. |
| shiftType | ShiftType | Опция смещения ячеек. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполнить некоторыми примерными данными
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // Определите область ячеек для вставки
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // Вставить диапазон и сместить ячейки вниз
            cells.InsertRange(area, ShiftType.Down);

            // Сохраните книгу
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Вставляет диапазон ячеек и смещает ячейки в соответствии с параметром смещения.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| область | CellArea | Сместить область. |
| shiftNumber | Int32 | Количество строк или столбцов для вставки. |
| shiftType | ShiftType | Опция смещения ячеек. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // Определите область ячеек для вставки (одна ячейка B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // Вставить диапазон, сместив ячейки вправо
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // Сохраните книгу
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


