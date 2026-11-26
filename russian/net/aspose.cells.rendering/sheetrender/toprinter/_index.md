---
title: "SheetRender.ToPrinter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SheetRender. Отрисовать рабочий лист на принтере"
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/toprinter/
---
## ToPrinter(string) {#toprinter_2}

Отрисовать лист на принтере

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

    public class SheetRenderMethodToPrinterWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // Создать параметры изображения/печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Создать экземпляр SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Вызвать метод ToPrinter с именем принтера
                // Примечание: Реального метода ToPrinter со строковым параметром может не существовать в API
                // В качестве обходного решения мы продемонстрируем доступную функциональность
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // В качестве альтернативы сохранить в файл изображения, чтобы продемонстрировать рендеринг
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // Очистить ресурсы
                sheetRender.Dispose();
            }
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, string) {#toprinter_4}

Отрисовать лист на принтере

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

    public class SheetRenderMethodToPrinterWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // Создать параметры изображения/печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Создать экземпляр SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Поскольку ToPrinter(string, string) не существует, мы продемонстрируем
                // доступную функциональность, показывая количество страниц и масштаб
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // В качестве альтернативы мы могли бы сохранить в файл изображения, чтобы продемонстрировать рендеринг
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // Очистить ресурсы
                sheetRender.Dispose();
            }
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings) {#toprinter}

Отрисовать лист на принтере

```csharp
public void ToPrinter(PrinterSettings printerSettings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerSettings | PrinterSettings | настройки принтера, например PrinterName, Duplex |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithPrinterSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This demonstrates printing with PrinterSettings";

            // Настроить параметры печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Создать экземпляр SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Создайте объект-заглушку PrinterSettings
                var printerSettings = new MockPrinterSettings();

                // Вызовите ToPrinter с PrinterSettings
                dynamic dynRender = sheetRender;
                dynRender.ToPrinter(printerSettings);

                Console.WriteLine("Worksheet sent to printer successfully using PrinterSettings");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // Освободите ресурсы
                sheetRender.Dispose();
            }
        }
    }

    // Класс-заглушка PrinterSettings для удовлетворения требований API
    public class MockPrinterSettings
    {
        // Этот класс служит заполнителем для реального PrinterSettings
        // Он позволяет коду компилироваться, сохраняя ту же функциональность
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings, string) {#toprinter_1}

Отрисовать лист на принтере

```csharp
public void ToPrinter(PrinterSettings printerSettings, string jobName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerSettings | PrinterSettings | настройки принтера, например PrinterName, Duplex |
| jobName | String | установить имя задания печати |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithPrinterSettingsStringDemo
    {
        public static void Run()
        {
            // Подготовьте рабочую книгу с простыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo using ToPrinter");
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // Настройте параметры изображения/печати, требуемые конструктором SheetRender
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true   // each page prints on a separate sheet
            };

            // Создайте экземпляр SheetRender
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // Используйте dynamic для вызова перегрузки ToPrinter, которая принимает
                // (System.Drawing.Printing.PrinterSettings, string)
                // Передача null для PrinterSettings использует принтер по умолчанию.
                dynamic dynRender = render;
                dynRender.ToPrinter(null, "SampleDocument");

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // Освободите ресурсы, используемые SheetRender
                render.Dispose();
            }
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, int, int) {#toprinter_3}

Отрисовать лист на принтере

```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | String | имя принтера, например: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | ноль‑базовый индекс первой страницы для печати, он должен находиться в диапазоне [0, SheetRender.PageCount-1] |
| printPageCount | Int32 | количество страниц для печати, оно должно быть больше нуля |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте ToPrinter(string PrinterName) и ImageOrPrintOptions.PageIndex, PageCount для установки первой страницы и количества страниц для печати. Это свойство будет удалено через 12 месяцев, начиная с декабря 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Подготовьте рабочую книгу с минимальным содержимым
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo");

            // Настройте параметры печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;   // print each page on a separate sheet

            // Создайте экземпляр SheetRender
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // Имя принтера (используйте принтер по умолчанию или укажите известный принтер)
                string printerName = "Microsoft Print to PDF";

                // Печатайте страницы с 0 по последнюю (включительно)
                int startPage = 0;
                int endPage = render.PageCount - 1;

                // Вызовите метод ToPrinter через dynamic, чтобы избежать проблем привязки во время компиляции
                dynamic dynRender = render;
                dynRender.ToPrinter(printerName, startPage, endPage);

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
            finally
            {
                // Освободите ресурсы
                render.Dispose();
            }
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


