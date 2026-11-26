---
title: "LoadOptions.LoadFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Фильтр, определяющий, как загружать данные"
type: docs
url: /ru/net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

Фильтр, указывающий, как загружать данные.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomLoadFilter : LoadFilter
    {
        public override void StartSheet(Worksheet sheet)
        {
            // Загружать данные только если лист видим
            if (sheet.IsVisible)
            {
                base.StartSheet(sheet);
            }
        }
    }

    public class LoadOptionsPropertyLoadFilterDemo
    {
        public static void Run()
        {
            // Создайте тестовую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "HiddenSheet";
            sheet.IsVisible = false;
            sheet.Cells["A1"].PutValue("This should not load");
            
            // Добавьте видимый лист
            Worksheet visibleSheet = workbook.Worksheets.Add("VisibleSheet");
            visibleSheet.Cells["A1"].PutValue("This will load");
            
            // Сохраните тестовый файл
            string filePath = "LoadFilterTest.xlsx";
            workbook.Save(filePath);
            workbook.Dispose();

            // Загрузите с пользовательским фильтром
            LoadOptions options = new LoadOptions();
            options.LoadFilter = new CustomLoadFilter();
            
            Workbook loadedWorkbook = new Workbook(filePath, options);
            
            // Проверьте, что загружен только видимый лист
            Console.WriteLine("Loaded Sheets:");
            foreach (Worksheet ws in loadedWorkbook.Worksheets)
            {
                Console.WriteLine($"- {ws.Name}: Visible={ws.IsVisible}");
                if (ws.IsVisible)
                {
                    Console.WriteLine($"  A1 Value: {ws.Cells["A1"].StringValue}");
                }
            }
            
            loadedWorkbook.Dispose();
        }
    }
}
```

### См. также

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


