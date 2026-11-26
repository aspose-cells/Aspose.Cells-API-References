---
title: "WorkbookSettings.CheckExcelRestriction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorkbookSettings property. Определяет, проверять ли ограничения Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValueString, и это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённое строковое значение как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако если вы задали значение, недопустимое для формата Excel, позже не следует сохранять рабочую книгу в формате Excel. В противном случае может возникнуть неожиданная ошибка в сгенерированном файле Excel."
type: docs
url: /ru/net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

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
    public class WorkbookSettingsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Отключить проверку ограничений Excel
            workbook.Settings.CheckExcelRestriction = false;
            
            // Вставьте строку, превышающую обычные ограничения Excel
            string longString = new string('a', 40000);
            workbook.Worksheets[0].Cells["A1"].PutValue(longString);
            
            // Сохраните и перезагрузите, чтобы убедиться, что ограничение обойдено
            string tempFile = Guid.NewGuid().ToString() + ".txt";
            workbook.Save(tempFile, new TxtSaveOptions());
            
            Workbook loadedWorkbook = new Workbook(tempFile, new LoadOptions { CheckExcelRestriction = false });
            Console.WriteLine("String length: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue.Length);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


