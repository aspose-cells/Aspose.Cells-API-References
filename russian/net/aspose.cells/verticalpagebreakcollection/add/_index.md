---
title: "VerticalPageBreakCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VerticalPageBreakCollection. Добавляет вертикальный разрыв страницы в коллекцию"
type: docs
url: /ru/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Добавляет вертикальный разрыв страницы в коллекцию.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки, начиная с нуля. |
| endRow | Int32 | Индекс конечной строки, начиная с нуля. |
| column | Int32 | Индекс столбца, начиная с нуля. |

### Возвращаемое значение

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Примечания

Этот метод используется для добавления вертикального разрыва страницы в пределах области печати.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
            
            // Продемонстрировать Add с параметрами (Int32, Int32, Int32)
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // Дополнительные примеры для контекста
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3

            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### См. также

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Добавляет вертикальный разрыв страницы в коллекцию.

```csharp
public int Add(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца ячейки, начиная с нуля. |

### Возвращаемое значение

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Примечания

Разрыв страницы добавлен в верхний левый угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Продемонстрировать метод Add с параметром Int32
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // Вывести детали добавленного разрыва страницы
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Добавляет вертикальный разрыв страницы в коллекцию.

```csharp
public int Add(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки ячейки, начиная с нуля. |
| column | Int32 | Индекс столбца ячейки, начиная с нуля. |

### Возвращаемое значение

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Примечания

Разрыв страницы добавлен в верхний левый угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию вертикальных разрывов страниц
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // Добавить вертикальные разрывы страниц в разных позициях столбцов
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // Добавить некоторые примерные данные для визуализации разрывов страниц
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // Сохраните книгу
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### См. также

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Добавляет вертикальный разрыв страницы в коллекцию.

```csharp
public int Add(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Возвращаемое значение

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Примечания

Разрыв страницы добавлен в верхний левый угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.VerticalPageBreaks.Add("G5");
            
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### См. также

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


