---
title: "Класс JsonConverter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.JsonConverter. Конвертер для преобразования между структурой данных json и другими форматами файлов электронных таблиц"
type: docs
url: /ru/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

Конвертер для преобразования JSON‑структуры данных в другие форматы файлов электронных таблиц.

```csharp
public class JsonConverter
```

## Методы

| Имя | Описание |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Преобразует между данными json и другими форматами файлов электронных таблиц. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Преобразует указанный файл шаблона между json и другими форматами. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // Преобразовать JSON в Excel с помощью Aspose.Cells.LowCode.JsonConverter
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


