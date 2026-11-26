---
title: "Класс DeleteOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DeleteOptions. Представляет настройки удаления строк/столбцов"
type: docs
url: /ru/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

Представляет настройку удаления строк/столбцов.

```csharp
public class DeleteOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Получает/задает монитор для отслеживания изменений, вызванных удалением. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Указывает, следует ли обновлять ссылки в других листах. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Отобразить исходные данные
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Создать DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Удалить вторую строку (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Отобразить данные после удаления
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Сохраните книгу
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


