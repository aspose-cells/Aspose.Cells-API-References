---
title: "SqlScriptSaveOptions.SheetIndexes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Представляет индексы экспортируемых листов"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/
---
## SqlScriptSaveOptions.SheetIndexes property

Представляет индексы экспортируемых листов.

```csharp
public int[] SheetIndexes { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с несколькими листами.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Заполните некоторыми данными все листы
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet worksheet = workbook.Worksheets[i];
                worksheet.Cells["A1"].PutValue("ID");
                worksheet.Cells["B1"].PutValue("Name");
                worksheet.Cells["A2"].PutValue(1);
                worksheet.Cells["B2"].PutValue("John");
                worksheet.Cells["A3"].PutValue(2);
                worksheet.Cells["B3"].PutValue("Jane");
            }

            // Создать экземпляр SqlScriptSaveOptions
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Отобразить текущие SheetIndexes (null означает все листы)
            Console.WriteLine("Initial SheetIndexes: " + 
                (options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));

            // Установить SheetIndexes для экспорта только первого и третьего листов (0 и 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Сохраните с параметрами.
            workbook.Save("SqlScriptExportSelectedSheets.sql", options);

            // Изменить SheetIndexes для экспорта только второго листа
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("SqlScriptExportSecondSheet.sql", options);

            // Установите SheetIndexes в null, чтобы экспортировать все листы
            options.SheetIndexes = null;
            workbook.Save("SqlScriptExportAllSheets.sql", options);
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


