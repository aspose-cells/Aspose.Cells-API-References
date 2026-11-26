---
title: "SaveOptions.SortExternalNames"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Указывает, следует ли сортировать внешне определённые имена перед сохранением файла"
type: docs
url: /ru/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Указывает, следует ли сортировать внешние определённые имена перед сохранением файла.

```csharp
public bool SortExternalNames { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создайте экземпляр OoxmlSaveOptions, который наследуется от SaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Отобразите значение по умолчанию свойства SortExternalNames
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // Установите SortExternalNames в true
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Сохраните книгу с указанными параметрами сохранения
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


