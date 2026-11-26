---
title: "PasteOptions.KeepOldTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PasteOptions. Сохраняет таблицы в диапазоне назначения"
type: docs
url: /ru/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Сохраняет таблицы в диапазоне назначения.

```csharp
public bool KeepOldTables { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создать пример листа с данными
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Создать экземпляр PasteOptions
                PasteOptions pasteOptions = new PasteOptions();

                // Отобразить значение свойства KeepOldTables по умолчанию
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // Установить KeepOldTables в true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Создать диапазоны для операции копирования
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // Копировать с опцией KeepOldTables
                targetRange.Copy(sourceRange, pasteOptions);

                // Сохраните книгу
                workbook.Save("KeepOldTablesDemo.xlsx");
                Console.WriteLine("Workbook saved with KeepOldTables option applied.");
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

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


