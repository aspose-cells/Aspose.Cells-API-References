---
title: "HorizontalPageBreakCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод HorizontalPageBreakCollection. Добавляет горизонтальный разрыв страницы в коллекцию"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Добавляет горизонтальный разрыв страницы в коллекцию.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки, начиная с нуля. |
| startColumn | Int32 | Индекс начального столбца, начиная с нуля. |
| endColumn | Int32 | Индекс конечного столбца, начиная с нуля. |

### Возвращаемое значение

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Примечания

Этот метод используется для добавления горизонтального разрыва страницы в пределах области печати.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Продемонстрировать метод Add с параметрами (Int32, Int32, Int32)
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### См. также

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Добавляет горизонтальный разрыв страницы в коллекцию.

```csharp
public int Add(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки ячейки, начиная с нуля. |

### Возвращаемое значение

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Примечания

Разрыв страницы добавлен в верхний левый угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить горизонтальные разрывы страниц, используя параметр Int32
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### См. также

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Добавляет горизонтальный разрыв страницы в коллекцию.

```csharp
public int Add(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки ячейки, начиная с нуля. |
| column | Int32 | Индекс столбца ячейки, начиная с нуля. |

### Возвращаемое значение

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Примечания

Разрыв страницы добавлен в верхний левый угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных, чтобы создать несколько строк
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Добавьте горизонтальные разрывы страниц в определённых строках
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // Сохраните книгу
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### См. также

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Добавляет горизонтальный разрыв страницы в коллекцию.

```csharp
public int Add(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Возвращаемое значение

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Примечания

Разрыв страницы добавлен в верхний левый угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте горизонтальный разрыв страницы в строке 4 (D5 — это строка 4 в индексе, начинающемся с нуля)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


