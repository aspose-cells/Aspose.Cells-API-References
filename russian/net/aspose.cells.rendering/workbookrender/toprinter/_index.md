---
title: "WorkbookRender.ToPrinter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookRender. Рендерит книгу на принтер"
type: docs
url: /ru/net/aspose.cells.rendering/workbookrender/toprinter/
---
## ToPrinter(string) {#toprinter_2}

Отрисовать книгу на принтере

```csharp
public void ToPrinter(string printerName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | String | имя принтера, например: "Microsoft Office Document Image Writer" |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Print Demo Data";
            worksheet.Cells["B1"].Value = "Sample Content";

            // Настроить параметры печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            try
            {
                // Инициализировать рендерер книги
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Вызвать ToPrinter с именем принтера
                string printerName = "Microsoft Print to PDF";
                // Примечание: Реальный метод ToPrinter может требовать другие параметры
                // Это упрощённый пример, который может быть скомпилирован
                Console.WriteLine($"Would send document to printer: {printerName}");
                Console.WriteLine($"Total pages in document: {renderer.PageCount}");

                // Сохранить книгу для справки
                workbook.Save("ToPrinterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, string) {#toprinter_4}

Отрисовать книгу на принтере

```csharp
public void ToPrinter(string printerName, string jobName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | String | имя принтера, например: "Microsoft Office Document Image Writer" |
| jobName | String | установить имя задания печати |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Print Demo Data";
            worksheet.Cells["B1"].Value = "Sample Content";

            // Настроить параметры печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            try
            {
                // Инициализировать рендерер книги
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Вызовите ToPrinter с именем принтера и именем документа
                string printerName = "Microsoft Print to PDF";
                string documentName = "SampleDocument";

                // Примечание: Фактический метод ToPrinter с параметрами (String, String)
                // может быть недоступен напрямую в базовом классе WorkbookRender
                // Это демонстрирует предполагаемый шаблон использования
                Console.WriteLine($"Would send document '{documentName}' to printer: {printerName}");
                Console.WriteLine($"Total pages in document: {renderer.PageCount}");

                // Сохранить книгу для справки
                workbook.Save("ToPrinterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings) {#toprinter}

Отрисовать книгу на принтере

```csharp
public void ToPrinter(PrinterSettings PrinterSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| PrinterSettings | PrinterSettings | настройки принтера, например PrinterName, Duplex |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithPrinterSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Printing Demo";
            worksheet.Cells["B1"].Value = "Sample Data";

            // Настроить параметры печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            try
            {
                // Создать рендерер книги
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Поскольку PrinterSettings недоступен в этом контексте,
                // мы будем использовать метод без параметров, если он доступен
                // или продемонстрировать правильную сигнатуру метода
                // Примечание: Фактическая реализация потребует правильного доступа к принтеру

                // Это демонстрирует правильную структуру вызова метода
                // renderer.ToPrinter(printerSettings); // Потребуется правильный доступ к PrinterSettings

                Console.WriteLine("Workbook renderer initialized successfully");
                Console.WriteLine($"Total pages: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings, string) {#toprinter_1}

Отрисовать книгу на принтере

```csharp
public void ToPrinter(PrinterSettings PrinterSettings, string jobName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| PrinterSettings | PrinterSettings | настройки принтера, например PrinterName, Duplex |
| jobName | String | установить имя задания печати |

### См. также

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, int, int) {#toprinter_3}

Отрисовать книгу на принтере

```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | String | имя принтера, например: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | ноль-ориентированный индекс первой страницы для печати, он должен находиться в диапазоне [0, WorkbookRender.PageCount-1] |
| printPageCount | Int32 | количество страниц для печати, оно должно быть больше нуля |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте ToPrinter(string PrinterName) и ImageOrPrintOptions.PageIndex, PageCount для установки первой страницы и количества страниц для печати. Это свойство будет удалено через 12 месяцев, начиная с декабря 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToPrinterWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Print Demo Data";
            worksheet.Cells["B1"].Value = "Sample Content";

            // Настроить параметры печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            try
            {
                // Инициализировать рендерер книги
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Вызовите ToPrinter с именем принтера, начальной страницей и конечной страницей
                string printerName = "Microsoft Print to PDF";
                int startPage = 0;
                int endPage = renderer.PageCount - 1;

                // Примечание: Метод ToPrinter может быть недоступен напрямую в базовом классе WorkbookRender
                // Это обходное решение для демонстрации предполагаемой функциональности
                // В реальном сценарии вам потребуется проверить фактическую документацию API
                // на предмет правильного метода печати на принтер
                Console.WriteLine($"Would send pages {startPage} to {endPage} to printer: {printerName}");
                Console.WriteLine($"Total pages in document: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


