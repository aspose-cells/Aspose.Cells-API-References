---
title: "HtmlSaveOptions.ExportHeadings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли заголовки строк и столбцов листов при сохранении в HTML‑файлы"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство HtmlSaveOptions.ExportRowColumnHeadings. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHeadingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Создайте параметры сохранения HTML и включите экспорт заголовков
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;

            // Сохранить как HTML с заголовками
            workbook.Save("output_with_headings.html", options);
            
            // Сохранить снова без заголовков для сравнения
            options.ExportHeadings = false;
            workbook.Save("output_without_headings.html", options);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


