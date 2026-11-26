---
title: "Worksheet.AutoFitRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Автоматически подгоняет высоту строки в прямоугольном диапазоне"
type: docs
url: /ru/net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Автоматически подгоняет высоту строки в прямоугольном диапазоне.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| endRow | Int32 | Индекс конечной строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endColumn | Int32 | Индекс конечного столбца. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RowCollection rows = worksheet.Cells.Rows;
            rows[0].Height = 20;
            rows[1].Height = 20;
            // Добавьте примерные данные в ячейки, чтобы продемонстрировать автоматическую подгонку строки
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
            worksheet.Cells["B1"].PutValue("Additional column with text");
            worksheet.Cells["A2"].PutValue("Shorter text");
            worksheet.Cells["B2"].PutValue("More text");
            
            try
            {
                Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");

                // Вызовите AutoFitRow с параметрами: startRow, endRow, startColumn, endColumn
                worksheet.AutoFitRow(0, 1, 0, 1);
                
                Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
                
                // Отобразите эффект, показывая высоты строк
                Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Автоматически подгоняет высоту строки.

```csharp
public void AutoFitRow(int rowIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |

### Примечания

AutoFitRow — неточная функция.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите длинный текст с переносом в ячейке A1
            worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Автоподгонка первой строки
            worksheet.AutoFitRow(0);

            // Сохраните книгу
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Автоматически подгоняет высоту строки.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |
| firstColumn | Int32 | Индекс первого столбца. |
| lastColumn | Int32 | Индекс последнего столбца. |

### Примечания

Этот метод автоматически подгоняет строку на основе содержимого в диапазоне ячеек внутри строки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные в ячейки, которые повлияют на высоту строки
            worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
            worksheet.Cells["B2"].PutValue("Additional text in another column");
            
            // Автоподгонка строки (строка 2) между столбцами 0 и 1 (A до B)
            worksheet.AutoFitRow(1, 0, 1);
            
            // Сохраните книгу
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Автоматически подгоняет высоту строки.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |
| firstColumn | Int32 | Индекс первого столбца. |
| lastColumn | Int32 | Индекс последнего столбца. |
| опции | AutoFitterOptions | Параметры автоподгонки |

### Примечания

Этот метод автоматически подгоняет строку на основе содержимого в диапазоне ячеек внутри строки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["B1"].PutValue("Another test string in column B");
            
            // Создать AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitMergedCells = true,
                IgnoreHidden = false,
                OnlyAuto = false
            };

            // Получить исходную высоту строки
            double originalHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"Original row height: {originalHeight}");

            // Автоподгонка первой строки
            worksheet.AutoFitRow(0, 0, 2, options);

            // Получить новую высоту строки
            double newHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"New row height after AutoFit: {newHeight}");

            // Сохраните книгу
            workbook.Save("AutoFitRowExample.xlsx");
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


