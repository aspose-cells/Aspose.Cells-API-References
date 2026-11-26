---
title: "EbookSaveOptions.EbookSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор EbookSaveOptions. Создаёт параметры для сохранения файла электронной книги"
type: docs
url: /ru/net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

Создает параметры для сохранения файла электронной книги.

```csharp
public EbookSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class EbookSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерное содержимое
            worksheet.Cells["A1"].PutValue("Ebook Test");
            worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
            
            // Создайте EbookSaveOptions с помощью конструктора
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            
            // Сохраните книгу Excel с помощью EbookSaveOptions (автоматически сохраняет как EPUB)
            workbook.Save("output.epub", saveOptions);
            
            Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
        }
    }
}
```

### См. также

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

Создает параметры для сохранения файла электронной книги.

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат файла. Должен быть Epub или Azw3. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Sample Ebook Content");
            
            try
            {
                // Вызовите метод #ctor с параметром SaveFormat
                EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
                
                // Установите дополнительные свойства при необходимости
                saveOptions.Encoding = System.Text.Encoding.UTF8;
                
                Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
                
                // Сохраните книгу с созданными параметрами
                workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


