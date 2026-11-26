---
title: "SaveOptions.CachedFileFolder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Папка для временных файлов, которые могут использоваться как кэш данных"
type: docs
url: /ru/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

Папка для временных файлов, которые могут использоваться как кэш данных.

```csharp
public string CachedFileFolder { get; set; }
```

### Примечания

Если папка не указана, значение по умолчанию для неё — [`GetCacheFolder`](../../cellshelper/getcachefolder/). Если её значение по умолчанию равно null или пусто, либо было указано как null или пусто, то при сохранении рабочей книги кэш‑файл использоваться не будет.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // Установить параметры сохранения с папкой кэш‑файлов
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // Сохраните книгу
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


