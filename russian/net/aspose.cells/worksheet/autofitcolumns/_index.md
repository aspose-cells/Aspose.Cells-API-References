---
title: "Worksheet.AutoFitColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet method. Автоматически подгоняет ширину всех столбцов в этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Автоматически подгоняет все столбцы в этом листе.

```csharp
public void AutoFitColumns()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("This is a test string");
            worksheet.Cells["B1"].PutValue("Another longer test string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            
            // Автоматически подгоните ширину всех столбцов в листе
            worksheet.AutoFitColumns();
            
            // Сохраните книгу
            workbook.Save("AutoFitColumnsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Автоматически подгоняет все столбцы в этом листе.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | AutoFitterOptions | Параметры автоматической подгонки |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Sample Text for AutoFit");
            worksheet.Cells["B1"].PutValue("Longer Sample Text for Testing AutoFitColumns");
            worksheet.Cells["C1"].PutValue(12345.6789);
            
            // Создать параметры авто‑подгонщика
            AutoFitterOptions options = new AutoFitterOptions();
            options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            
            // Автоподгонка столбцов с параметрами
            worksheet.AutoFitColumns(options);
            
            // Сохраните книгу
            workbook.Save("AutoFitColumnsWithOptions.xlsx");
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int) {#autofitcolumns_2}

Автоматически подгоняет ширину столбцов.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstColumn | Int32 | Индекс первого столбца. |
| lastColumn | Int32 | Индекс последнего столбца. |

### Примечания

AutoFitColumn — неточная функция.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные для демонстрации автоподгонки
            sheet.Cells["A1"].PutValue("Short");
            sheet.Cells["B1"].PutValue("Medium length text");
            sheet.Cells["C1"].PutValue("Very very long text that needs column width adjustment");
            sheet.Cells["D1"].PutValue("Another example with different length");

            // Автоподгонка столбцов с индекса 0 до 3
            sheet.AutoFitColumns(0, 3);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Автоматически подгоняет ширину столбцов.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstColumn | Int32 | Индекс первого столбца. |
| lastColumn | Int32 | Индекс последнего столбца. |
| опции | AutoFitterOptions | Параметры автоматической подгонки |

### Примечания

AutoFitColumn — неточная функция.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
            worksheet.Cells["C1"].PutValue("Another example with different length");

            // Создайте AutoFitterOptions с конкретными настройками
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Вызовите AutoFitColumns с параметрами (firstColumn, lastColumn, options)
                worksheet.AutoFitColumns(0, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
                
                // Отобразите эффект, показывая ширину столбцов
                Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Автоматически подгоняет ширину столбцов.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Индекс первой строки. |
| firstColumn | Int32 | Индекс первого столбца. |
| lastRow | Int32 | Индекс последней строки. |
| lastColumn | Int32 | Индекс последнего столбца. |

### Примечания

AutoFitColumn — неточная функция.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми данными для демонстрации
            worksheet.Cells["A1"].PutValue("Short");
            worksheet.Cells["B1"].PutValue("Medium length text");
            worksheet.Cells["C1"].PutValue("Very very long text that needs more column width");
            
            // Автоподгонка столбцов с столбца 0 (A) до столбца 2 (C), с первой строкой 0 и последней строкой 0
            worksheet.AutoFitColumns(0, 2, 0, 0);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Автоматически подгоняет ширину столбцов.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Индекс первой строки. |
| firstColumn | Int32 | Индекс первого столбца. |
| lastRow | Int32 | Индекс последней строки. |
| lastColumn | Int32 | Индекс последнего столбца. |
| опции | AutoFitterOptions | Параметры автоматической подгонки |

### Примечания

AutoFitColumn — неточная функция.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните ячейки примерными данными, требующими корректировки ширины столбцов
            worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
            worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            worksheet.Cells["A2"].PutValue(12345.6789);
            worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
            worksheet.Cells["C2"].PutValue(true);

            // Создайте AutoFitterOptions с конкретными настройками
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // Вызовите AutoFitColumns с конкретными параметрами (firstRow, firstColumn, lastRow, lastColumn, options)
                worksheet.AutoFitColumns(0, 0, 1, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
                
                // Отобразите ширину столбцов после автоподгонки
                Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


