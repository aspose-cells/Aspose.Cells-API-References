---
title: "DbfSaveOptions.ExportAsString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DbfSaveOptions. Указывает, экспортировать ли как строковое значение"
type: docs
url: /ru/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

Указывает, экспортировать ли как строковое значение

```csharp
public bool ExportAsString { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные со смешанными типами
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // Создать экземпляр DbfSaveOptions
            DbfSaveOptions options = new DbfSaveOptions();

            // Отобразить текущее значение ExportAsString
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Установить ExportAsString в true (все значения будут экспортированы как строки)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Сохранить с ExportAsString = true
            workbook.Save("ExportAsStringTrue.dbf", options);

            // Установить ExportAsString в false (значения сохранят свои исходные типы)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Сохранить с ExportAsString = false
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### См. также

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


