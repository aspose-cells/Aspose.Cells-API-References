---
title: "Перечисление OpenDocumentFormatVersionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. Тип версии формата Open Document"
type: docs
url: /ru/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Тип версии формата Open Document.

```csharp
public enum OpenDocumentFormatVersionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет строгих. |
| Odf11 | `1` | Версия ODF 1.1 |
| Odf12 | `2` | Версия ODF 1.2 |
| Odf13 | `3` | Версия ODF 1.3 |
| Odf14 | `4` | Версия ODF 1.4 |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OpenDocumentFormatVersionTypeDemo
    {
        public static void OpenDocumentFormatVersionTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Создайте OdsSaveOptions и установите версию ODF
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Сохраните книгу в формате ODS с указанной версией ODF
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


