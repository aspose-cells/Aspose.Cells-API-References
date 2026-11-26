---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocxSaveOptions. Сохраняет все графические objecgts как редактируемые формы в файле Word. Так вы можете редактировать их в Word"
type: docs
url: /ru/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Сохранить все графические objecgts как редактируемые формы в файле Word. Так вы можете редактировать их в Word.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [`SaveAsEditableShapes`](../saveaseditableshapes/). Это свойство будет удалено через 6 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // Создайте объект рабочей книги и откройте шаблонный файл Excel
            Workbook workbook = new Workbook("example.xlsx");

            // Инициализируйте DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // Установите свойство SaveAsEditableShaps в true
            saveOptions.SaveAsEditableShaps = true;

            // Сохраните рабочую книгу как DOCX с указанными параметрами
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### См. также

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


