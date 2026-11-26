---
title: "Класс SheetSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.SheetSet. Описывает набор листов"
type: docs
url: /ru/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

Описывает набор листов.

```csharp
public class SheetSet
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Создаёт набор листов на основе точных индексов листов. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Создаёт набор листов на основе точных имён листов. |

## Свойства

| Имя | Описание |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Получает набор с активным листом книги. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Получает набор со всеми листами книги в их исходном порядке. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Получает набор с видимыми листами книги в их исходном порядке. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // Создайте объект PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Установите свойство SheetSet, чтобы включать только активный лист
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Сохраните книгу в PDF‑файл
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // Установите свойство SheetSet, чтобы включить все видимые листы
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Сохраните книгу в PDF‑файл
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // Установите свойство SheetSet, чтобы включить все листы
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Сохраните книгу в PDF‑файл
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


