---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Каталог, в который будут сохраняться вложенные файлы"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

Каталог, в который будут сохраняться вложенные файлы.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо него используйте свойство HtmlLoadOptions.StreamProvider. Это свойство будет удалено через 12 месяцев, начиная с декабря 2014 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Создать экземпляр HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Установить каталог для вложенных файлов
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // Загрузить HTML‑файл в книгу Workbook, используя указанные параметры
            Workbook workbook = new Workbook("input.html", options);

            // Сохраните Workbook в файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


