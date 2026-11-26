---
title: "Cells.CopyColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Копирует данные и форматы целого столбца"
type: docs
url: /ru/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Копирует данные и форматы целого столбца.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | Int32 | Индекс исходного столбца. |
| destinationColumnIndex | Int32 | Индекс целевого столбца. |
| columnNumber | Int32 | Номер скопированного столбца. |
| pasteOptions | PasteOptions | параметры вставки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Создать другую книгу в качестве назначения
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // Копировать столбцы только с форматированием
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // Сохраните книгу
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

Копирует данные и форматы целых столбцов.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | Int32 | Индекс исходного столбца. |
| destinationColumnIndex | Int32 | Индекс целевого столбца. |
| columnNumber | Int32 | Номер скопированного столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавить примерные данные в столбцы
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // Копировать столбцы от индекса 1 (B) до индекса 3 (D), скопировать 1 столбец
            cells.CopyColumns(cells, 1, 3, 1);

            // Сохраните книгу
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Копирует данные и форматы всех столбцов.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceCells | Ячейки | Объект Source Cells содержит данные и форматы для копирования. |
| sourceColumnIndex | Int32 | Индекс исходного столбца. |
| sourceTotalColumns | Int32 | Количество исходных столбцов. |
| destinationColumnIndex | Int32 | Индекс целевого столбца. |
| destinationTotalColumns | Int32 | Количество целевых столбцов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполнить исходные столбцы (столбцы 0 и 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // Копировать 2 столбца от индекса 0 до целевого индекса 3, вставляя 2 столбца
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // Проверить копирование, проверив целевые столбцы (3 и 4)
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


