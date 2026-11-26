---
title: "Перечисление DirectoryType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DirectoryType. Представляет тип каталога имени файла"
type: docs
url: /ru/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

Представляет тип каталога имени файла.

```csharp
public enum DirectoryType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Volume | `0` | Представляет букву диска MS-DOS. За ней следует буква диска. Или имена файлов UNC, такие как \\server\share\myfile.xls |
| SameVolume | `1` | Указывает, что исходная рабочая книга находится на том же диске, что и зависимая рабочая книга (буква диска опущена) |
| DownDirectory | `2` | Указывает, что исходная рабочая книга находится в подкаталоге текущего каталога. |
| UpDirectory | `3` | Указывает, что исходная рабочая книга находится в родительском каталоге текущего каталога. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Добавить внешнюю ссылку в рабочую книгу
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // Добавить внешнюю ссылку с DirectoryType.Volume
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // Получить добавленную внешнюю ссылку
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // Вывести детали внешней ссылки
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // Сохраните книгу
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


