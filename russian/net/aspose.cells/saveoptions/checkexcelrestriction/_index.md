---
title: "SaveOptions.CheckExcelRestriction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 K. Если ввести значение длиннее 32 K, оно будет усечено"
type: docs
url: /ru/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Отключить проверку ограничений Excel
            workbook.Settings.CheckExcelRestriction = false;

            // Получите доступ к первому листу и ячейкам
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Создайте строку, превышающую обычный лимит Excel
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Поместите длинную строку в ячейку A1
            cells["A1"].PutValue(longString);

            // Настройте параметры сохранения для обхода ограничений
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // Сохраните книгу
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // Загрузите сохранённый файл с отключёнными ограничениями
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // Проверьте, что длинная строка сохранена
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


