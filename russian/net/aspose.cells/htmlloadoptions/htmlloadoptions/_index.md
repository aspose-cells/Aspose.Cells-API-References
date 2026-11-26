---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор HtmlLoadOptions. Создаёт параметры загрузки файла"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Создаёт параметры загрузки файла.

```csharp
public HtmlLoadOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки HTML с помощью конструктора
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // Загрузите HTML‑файл с использованием параметров
            Workbook workbook = new Workbook("example.html", loadOptions);

            // Получите доступ к данным из загруженного HTML
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Создаёт параметры загрузки файла.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | LoadFormat | Формат загрузки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр HtmlLoadOptions, используя конструктор с параметром LoadFormat
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // Установите некоторые свойства HtmlLoadOptions
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Создайте книгу, используя параметры загрузки
                Workbook workbook = new Workbook("input.html", loadOptions);

                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];

                // Отобразить некоторую информацию о загруженном HTML
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Сохраните книгу
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


