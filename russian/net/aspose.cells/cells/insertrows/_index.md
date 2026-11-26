---
title: "Cells.InsertRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Вставляет несколько строк в лист"
type: docs
url: /ru/net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

Вставляет несколько строк в лист.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |
| totalRows | Int32 | Количество строк для вставки. |
| updateReference | Boolean | Указывает, будут ли обновляться ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Вставить строку с индексом 2 (она станет новой строкой 3)
            worksheet.Cells.InsertRows(2, 1, true);
            
            // Добавить данные в вставленную строку
            worksheet.Cells["A3"].PutValue("Inserted Data");
            
            // Сохраните книгу
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

Вставляет несколько строк в лист.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |
| totalRows | Int32 | Количество строк для вставки. |
| опции | InsertOptions | Параметры операции вставки. |

### Примеры

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми образцовыми данными
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Вставить 3 строки по индексу строки 5 с указанными параметрами
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            workbook.Save("InsertRowsWithOptions.xlsx");
        }
    }
}
```

### См. также

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

Вставляет несколько строк в лист.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |
| totalRows | Int32 | Количество строк для вставки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте некоторые образцы данных.
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Data1");
            cells["B2"].PutValue("Data2");
            cells["A3"].PutValue("Data3");
            cells["B3"].PutValue("Data4");

            // Вставить 2 строки по индексу строки 2
            cells.InsertRows(2, 2);

            // Проверить, что вставленные строки пусты
            Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
            Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"

            // Сохраните книгу
            workbook.Save("InsertRowsDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


