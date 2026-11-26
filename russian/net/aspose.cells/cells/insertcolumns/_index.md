---
title: "Cells.InsertColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Вставляет несколько столбцов в лист"
type: docs
url: /ru/net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

Вставляет несколько столбцов в лист.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца. |
| totalColumns | Int32 | Количество столбцов. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Вставить 3 столбца, начиная с индекса столбца 1 (второй столбец)
            worksheet.Cells.InsertColumns(1, 3);
            
            // Добавьте примерные данные, чтобы продемонстрировать вставленные столбцы
            worksheet.Cells["A1"].PutValue("Original Column");
            worksheet.Cells["B1"].PutValue("Inserted Column 1");
            worksheet.Cells["C1"].PutValue("Inserted Column 2");
            worksheet.Cells["D1"].PutValue("Inserted Column 3");
            worksheet.Cells["E1"].PutValue("Original Column 2");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

Вставляет несколько столбцов в лист.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца. |
| totalColumns | Int32 | Количество столбцов. |
| updateReference | Boolean | Указывает, будут ли обновляться ссылки в других листах. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Вставить 3 столбца в индекс столбца 2 (нумерация с нуля), сдвигая существующие столбцы вправо
            worksheet.Cells.InsertColumns(2, 3, true);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

Вставляет несколько столбцов в лист.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца. |
| totalColumns | Int32 | Количество столбцов. |
| опции | InsertOptions | Параметры операции вставки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Создать параметры вставки
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.Clear;

            // Вставить столбец в индекс 1 (второй столбец)
            worksheet.Cells.InsertColumns(1, 1, options);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


