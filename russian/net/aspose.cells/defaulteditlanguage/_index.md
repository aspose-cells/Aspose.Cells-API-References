---
title: "Перечисление DefaultEditLanguage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DefaultEditLanguage. Представляет язык редактирования по умолчанию"
type: docs
url: /ru/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

Представляет язык редактирования по умолчанию.

```csharp
public enum DefaultEditLanguage
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Auto | `0` | Представляет автоматическое определение языка редактирования в соответствии с самим текстом. |
| English | `1` | Представляет английский язык. |
| CJK | `2` | Представляет китайский, японский и корейский языки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте AutoFitterOptions и установите DefaultEditLanguage
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Примените автоматическую подгонку строк с указанными параметрами
            worksheet.AutoFitRows(autoFitterOptions);

            // Сохраните книгу
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Выведите установленный DefaultEditLanguage в консоль
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


