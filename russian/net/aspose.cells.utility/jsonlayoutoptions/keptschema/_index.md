---
title: "JsonLayoutOptions.KeptSchema"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Указывает, сохраняется ли схема этого JSON"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/keptschema/
---
## JsonLayoutOptions.KeptSchema property

Указывает, сохранять ли схему этого JSON.

```csharp
public bool KeptSchema { get; set; }
```

### Примечания

Иногда мы сохраняем файл в JSON после загрузки файла JSON.

### Примеры

```csharp
using System;
using System.IO;
using System.Text.Json;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyKeptSchemaDemo
    {
        public class Data
        {
            public string RootProperty { get; set; }
            public Payload Payload { get; set; }
        }

        public class Payload
        {
            public ArrayData[] Array { get; set; }
            public string PayloadProperty { get; set; }
            public PayloadStruct PayloadStruct { get; set; }
        }

        public class ArrayData
        {
            public string ArrayProperty { get; set; }
        }

        public struct PayloadStruct
        {
            public string PayloadProperty1 { get; set; }
            public string PayloadProperty2 { get; set; }
        }

        public static void Run()
        {
            // Создать примерные данные
            var data = new Data()
            {
                RootProperty = "RootValue",
                Payload = new Payload()
                {
                    Array = new[]
                    {
                        new ArrayData() { ArrayProperty = "item1" },
                        new ArrayData() { ArrayProperty = "item2" }
                    },
                    PayloadProperty = "PayloadValue",
                    PayloadStruct = new PayloadStruct()
                    {
                        PayloadProperty1 = "struct1",
                        PayloadProperty2 = "struct2"
                    }
                }
            };

            // Сериализовать в JSON с использованием System.Text.Json
            string json = JsonSerializer.Serialize(new[] { data });

            // Создать книгу и импортировать JSON
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.KeptSchema = true; // Demonstrate KeptSchema usage
            
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, layoutOptions);

            // Сохранить и вывести результаты
            string outputPath = "output/";
            Directory.CreateDirectory(outputPath);
            
            workbook.Save(outputPath + "KeptSchemaDemo.xlsx", SaveFormat.Xlsx);
            workbook.Save(outputPath + "KeptSchemaDemo.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true
            });

            Console.WriteLine("Files saved successfully. Check output directory.");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


