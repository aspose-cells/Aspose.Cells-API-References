---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Указывает, следует ли проверять совместимость шрифта для каждого символа в тексте.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Примечания

Значение по умолчанию — true. Отключение этого свойства может дать лучшую производительность. Однако, если шрифт текста/символа по умолчанию или указанный шрифт нельзя использовать для его рендеринга, в сгенерированном PDF могут появиться нечитаемые символы (например, блоки). В такой ситуации пользователь должен оставить это свойство включённым (true), чтобы можно было искать альтернативный шрифт и использовать его для рендеринга текста вместо этого;

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // Создайте параметры постраничного сохранения
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Продемонстрируйте свойство CheckFontCompatibility
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // Установите другие необходимые свойства
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // Сохраните документ с указанными параметрами
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


