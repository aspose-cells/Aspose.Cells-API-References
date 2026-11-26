---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Получает имя листа по умолчанию для автоматического добавления листа. По умолчанию — Sheet"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Получает имя листа по умолчанию для автоматического добавления листа. По умолчанию "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Возвращаемое значение

имя листа по умолчанию для автоматического добавления листа

### Примечания

Имя автоматически добавленного (например, с помощью [`Add`](../../worksheetcollection/add/)) листа будет состоять из указанного имени плюс порядковый номер. Например, пользователь из Германии может захотеть, чтобы имя листа было "Tabellenblatt2" вместо "Sheet2". Тогда пользователь может реализовать этот метод, чтобы он возвращал "Tabellenblatt".

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить пользовательские настройки глобализации
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Получить имя листа по умолчанию из пользовательских настроек глобализации
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // Добавить новый лист, чтобы продемонстрировать именование на основе пользовательского значения по умолчанию
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // Реализация пользовательских настроек глобализации
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


