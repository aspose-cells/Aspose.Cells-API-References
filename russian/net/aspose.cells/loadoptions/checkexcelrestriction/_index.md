---
title: "LoadOptions.CheckExcelRestriction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиннее 32 КБ. Когда вы вводите значение длиннее 32 КБ, например с помощью Cell.PutValuestring, если это свойство истинно, вы получите исключение. Если свойство ложно, мы примем введённое строковое значение как значение ячейки, чтобы позже вы могли вывести полное строковое значение для других форматов файлов, таких как CSV. Однако если вы задали значение, которое недействительно для формата файла Excel, вы не должны сохранять рабочую книгу в формате Excel позже. Иначе может возникнуть непредвиденная ошибка в сгенерированном файле Excel."
type: docs
url: /ru/net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиннее 32 КБ, например через Cell.PutValue(string), если это свойство равно true, вы получите исключение. Если свойство равно false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, позже не следует сохранять рабочую книгу в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Отключить проверку ограничений Excel
            workbook.Settings.CheckExcelRestriction = false;

            // Получите доступ к первому листу и ячейкам
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Создайте строку, превышающую обычный лимит Excel (32767 символов)
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Поместите длинную строку в ячейку A1
            cells["A1"].PutValue(longString);
            
            // Сохранить с отключённой проверкой ограничений
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;
            workbook.Save("output.xlsx", saveOptions);
            
            // Загрузить с отключённой проверкой ограничений
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output.xlsx", loadOptions);
            
            // Проверьте, что длинная строка сохранена
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("String length: " + loadedValue.Length);
            Console.WriteLine("String matches: " + loadedValue.Equals(longString));
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


