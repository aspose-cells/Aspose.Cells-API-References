---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор DbfSaveOptions. Параметры сохранения файла .dbf"
type: docs
url: /ru/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

Параметры сохранения файла .dbf.

```csharp
public DbfSaveOptions()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Создать экземпляр DbfSaveOptions с помощью конструктора
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // Установить свойства параметров сохранения
                saveOptions.ExportAsString = true;
                
                // Сохраните книгу с параметрами сохранения DBF
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


