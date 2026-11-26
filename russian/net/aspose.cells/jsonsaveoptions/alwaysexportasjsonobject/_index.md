---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Указывает, следует ли всегда экспортировать Excel в JSON как объект, даже если в файле только один лист"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Указывает, следует ли всегда экспортировать Excel в JSON как объект, даже если в файле только один лист.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // Создайте пример книги с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Установите некоторые примерные данные в первый лист
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // Настройте параметры сохранения JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Сохранить в файл JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // Отобразите сохранённое содержимое JSON
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


