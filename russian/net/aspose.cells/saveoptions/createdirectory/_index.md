---
title: "SaveOptions.CreateDirectory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла"
type: docs
url: /ru/net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

```csharp
public bool CreateDirectory { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCreateDirectoryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Установить параметры сохранения с включённым CreateDirectory
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.CreateDirectory = true;

            // Сохранить книгу в новый каталог (будет создан автоматически)
            string outputPath = "OutputDirectory/example.xls";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved successfully with directory creation.");
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


