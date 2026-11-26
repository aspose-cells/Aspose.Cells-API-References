---
title: "Cells.ClearFormats"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Очищает форматирование диапазона"
type: docs
url: /ru/net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Очищает форматирование диапазона.

```csharp
public void ClearFormats(CellArea range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | CellArea | Диапазон для очистки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерные данные с форматированием
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // Применить форматирование к ячейкам
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            
            for (int row = formatArea.StartRow; row <= formatArea.EndRow; row++)
            {
                for (int col = formatArea.StartColumn; col <= formatArea.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Formatted {row},{col}");
                    cells[row, col].SetStyle(style);
                }
            }

            // Определить область очистки
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // Очистить форматирование из центральной ячейки
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // Обновить значение очищенной ячейки, чтобы показать эффект
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearFormats(int, int, int, int) {#clearformats_1}

Очищает форматирование диапазона.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endRow | Int32 | Индекс конечной строки. |
| endColumn | Int32 | Индекс конечного столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearFormatsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Применить стили к некоторым ячейкам
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            cells[0, 0].SetStyle(style);
            cells[0, 10].SetStyle(style);
            cells[10, 0].SetStyle(style);
            cells[10, 10].SetStyle(style);

            // Очистить форматирование из конкретного диапазона (строки 5-15, столбцы 5-15)
            cells.ClearFormats(5, 5, 15, 15);

            // Сохраните книгу
            workbook.Save("ClearedFormats.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


