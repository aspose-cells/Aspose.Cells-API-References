---
title: "Cells.CopyRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Копирует данные и форматы некоторых целых строк"
type: docs
url: /ru/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Копирует данные и форматы некоторых целых строк.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | Int32 | Индекс исходной строки. |
| destinationRowIndex | Int32 | Индекс целевой строки. |
| rowNumber | Int32 | Номер скопированной строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // Добавьте некоторые примерные данные в исходную книгу
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // Получите ячейки из обеих книг
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // Скопируйте все строки из источника в назначение, начиная с строки 0 в назначении
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // Сохранить результат
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Копирует данные и форматы некоторых целых строк.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | Int32 | Индекс исходной строки. |
| destinationRowIndex | Int32 | Индекс целевой строки. |
| rowNumber | Int32 | Номер скопированной строки. |
| copyOptions | CopyOptions | Параметры копирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные и гиперссылки
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Вставьте пустую строку в строку 5
            worksheet.Cells.InsertRows(5, 1);

            // Скопировать строку 4 в строку 5 без CopyOptions
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // Сбросить лист
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Вставить пустую строку в строку 5 снова
            worksheet.Cells.InsertRows(5, 1);

            // Скопировать строку 4 в строку 5 с CopyOptions
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### См. также

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Копирует данные и форматы некоторых целых строк.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells0 | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceRowIndex | Int32 | Индекс исходной строки. |
| destinationRowIndex | Int32 | Индекс целевой строки. |
| rowNumber | Int32 | Номер скопированной строки. |
| copyOptions | CopyOptions | Параметры копирования. |
| pasteOptions | PasteOptions | параметры вставки. |

### См. также

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


