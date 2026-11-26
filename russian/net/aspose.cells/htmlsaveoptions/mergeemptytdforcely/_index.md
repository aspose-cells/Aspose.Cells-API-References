---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, следует ли принудительно объединять пустые элементы TD при экспорте файла в html. Размер html‑файла будет значительно уменьшен после установки значения в true. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, пожалуйста, оставьте значение по умолчанию."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Указывает, следует ли принудительно объединять пустые элементы TD при экспорте файла в html. Размер html‑файла будет значительно уменьшен после установки значения в true. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel или экспортировать идеальные линии сетки при сохранении файла в html, пожалуйста, оставьте значение по умолчанию.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // Создайте пример рабочей книги с пустыми ячейками
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте несколько пустых ячеек в листе
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // Ячейка B2 намеренно оставлена пустой
            
            // Сохраните с включённым MergeEmptyTdForcely
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // Сохраните без MergeEmptyTdForcely для сравнения
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


