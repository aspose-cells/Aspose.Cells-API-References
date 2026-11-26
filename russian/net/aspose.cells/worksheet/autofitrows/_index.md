---
title: "Worksheet.AutoFitRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Автоматически подгоняет высоту всех строк в этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Автоматически подгоняет все строки в этом листе.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | AutoFitterOptions | Параметры автоподгонки |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерные данные и форматирование
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // Объединить ячейки, чтобы продемонстрировать автоматическую подгонку объединённых ячеек
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // Автоматически подогнать строки с определёнными параметрами
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // Сохраните книгу
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows(int, int) {#autofitrows_3}

Автоматически подгоняет высоту строки в диапазоне.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| endRow | Int32 | Индекс конечной строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить ячейки примерными данными и стилями
            for (int i = 0; i <= 8; i++)
            {
                Cell cell = cells[i, i];
                cell.Value = "Sample text for row " + i;
                
                if (i % 2 == 0)
                {
                    Style style = cell.GetStyle();
                    style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
                    cell.SetStyle(style);
                }
            }

            // Автоматически подогнать строки с индекса 0 до 8
            sheet.AutoFitRows(0, 8);

            // Вывести полученные высоты строк
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Автоматически подгоняет высоту строки в диапазоне.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| endRow | Int32 | Индекс конечной строки. |
| опции | AutoFitterOptions | Параметры авто‑подгонщика. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // Создать параметры авто‑подгонщика
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // Автоматически подогнать строки 0‑1 с параметрами
            worksheet.AutoFitRows(0, 1, options);
            
            // Сохраните книгу
            workbook.Save("AutoFitRowsDemo.xlsx");
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

## AutoFitRows() {#autofitrows}

Автоматически подгоняет все строки в этом листе.

```csharp
public void AutoFitRows()
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // Автоматически подогнать строки
            worksheet.AutoFitRows();
            
            // Автоматически подогнать столбцы для лучшей видимости
            worksheet.AutoFitColumns();
            
            // Сохраните книгу
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Автоматически подгоняет все строки в этом листе.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| onlyAuto | Boolean | True, только автоматически подгоняет высоту строки, когда высота строки не задана вручную. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерный текст в ячейки, чтобы продемонстрировать автоматическую подгонку строк
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // Автоматически подогнать строки с учётом автоматического объединения
            worksheet.AutoFitRows(true);
            
            // Сохраните книгу
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


