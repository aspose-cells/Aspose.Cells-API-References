---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор EbookLoadOptions. Создаёт параметр для загрузки файла ebook"
type: docs
url: /ru/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

Создаёт параметр для загрузки файла электронной книги.

```csharp
public EbookLoadOptions()
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте экземпляр EbookLoadOptions, используя конструктор
            EbookLoadOptions options = new EbookLoadOptions();

            // Установите некоторые базовые свойства
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Загрузите файл ebook с указанными параметрами
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Сохранить как файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

Создаёт параметр загрузки файла электронной книги.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | LoadFormat | Формат загрузки |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр EbookLoadOptions с параметром LoadFormat
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Отобразить подтверждение
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Пример использования: загрузите книгу с этими параметрами
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Сохранить результат
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


