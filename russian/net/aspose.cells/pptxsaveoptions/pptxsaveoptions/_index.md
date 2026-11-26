---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор PptxSaveOptions. Представляет параметры сохранения pptx"
type: docs
url: /ru/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Представляет параметры сохранения pptx.

```csharp
public PptxSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Скрыть вторую строку
            worksheet.Cells.Rows[1].IsHidden = true;

            // Создайте PptxSaveOptions с помощью конструктора
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // Сохраните книгу в PPTX с параметрами
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### См. также

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Представляет параметры сохранения файла .pptx.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveAsImage | Boolean | Если True, книга будет преобразована в несколько изображений файла .pptx. Если False, книга будет преобразована в несколько таблиц файла .pptx. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Вызовите метод #ctor с булевым параметром
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Установить дополнительные свойства
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Сохраните книгу с параметрами PPTX
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


