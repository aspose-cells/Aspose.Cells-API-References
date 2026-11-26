---
title: "Перечисление ExternalLinkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalLinkType. Представляет тип внешней ссылки"
type: docs
url: /ru/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

Представляет тип внешней ссылки.

```csharp
public enum ExternalLinkType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DDELink | `0` | Представляет DDE‑ссылку. |
| External | `1` | Представляет внешнюю ссылку. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // Открыть файл с внешними ссылками
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Получить внешнюю ссылку 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Отобразить тип внешней ссылки
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Изменить источник данных внешней ссылки
            externalLink.DataSource = "d:\\link.xls";

            // Сохраните книгу
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // Перечисление, представляющее тип внешней ссылки
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


