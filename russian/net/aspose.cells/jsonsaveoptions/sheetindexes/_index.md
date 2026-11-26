---
title: "JsonSaveOptions.SheetIndexes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Представляет индексы экспортируемых листов"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

Представляет индексы экспортируемых листов.

```csharp
public int[] SheetIndexes { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с несколькими листами.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Заполните некоторыми данными каждый лист
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // Создайте экземпляр JsonSaveOptions
            JsonSaveOptions options = new JsonSaveOptions();

            // Отобразите текущие SheetIndexes (по умолчанию null — экспортируются все листы)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // Установите экспорт только первого и третьего листов (индексы 0 и 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Сохранить в JSON с выбранными листами
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // Проверьте, загрузив JSON
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // Изменить на экспорт только второго листа (индекс 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // Проверьте экспорт одного листа
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


