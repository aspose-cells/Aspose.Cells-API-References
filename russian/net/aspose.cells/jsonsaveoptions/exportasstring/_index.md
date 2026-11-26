---
title: "JsonSaveOptions.ExportAsString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Экспортирует строковое значение ячеек в json"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/exportasstring/
---
## JsonSaveOptions.ExportAsString property

Экспортирует строковое значение ячеек в JSON.

```csharp
public bool ExportAsString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Создать пример данных с числовыми значениями
            cells["A1"].PutValue("Age");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue(30);
            cells["B2"].PutValue(95.5);

            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            string jsonOutput = JsonUtility.ExportRangeToJson(cells.CreateRange("A1:B2"), exportOptions);
            Console.WriteLine("Exported JSON with ExportAsString=true:\n" + jsonOutput);
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


