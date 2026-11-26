---
title: "Класс ExternalLink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ExternalLink. Представляет внешнюю ссылку в рабочей книге"
type: docs
url: /ru/net/aspose.cells/externallink/
---
## ExternalLink class

Представляет внешнюю ссылку в книге.

```csharp
public class ExternalLink
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Представляет источник данных внешней ссылки. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Указывает, ссылаются ли другие элементы на эту внешнюю ссылку. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Указывает, видна ли эта внешняя ссылка в MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Представляет сохранённый источник данных внешней ссылки. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Получить тип пути этой внешней ссылки |
| [Type](../../aspose.cells/externallink/type/) { get; } | Получает тип внешней ссылки. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Добавляет внешнее имя. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // Открыть файл с внешними ссылками
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Получить внешнюю ссылку 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Отобразить свойства внешней ссылки
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Изменить источник данных внешней ссылки
            externalLink.DataSource = "d:\\linktest.xls";

            // Добавить внешнее имя к внешней ссылке
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Сохраните книгу
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


