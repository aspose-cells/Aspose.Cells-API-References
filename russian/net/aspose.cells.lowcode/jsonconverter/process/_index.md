---
title: "JsonConverter.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод JsonConverter. Преобразует указанный файл шаблона между json и другими форматами"
type: docs
url: /ru/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

Преобразует указанный файл шаблона между json и другими форматами.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | String | Файл шаблона для преобразования |
| resultFile | String | Полученный файл |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class JsonConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Создайте пример данных JSON и запишите их во временный файл
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // Обрабатывайте файлы напрямую, используя статический метод JsonConverter
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // Очистите временный файл JSON
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### См. также

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Преобразует между данными json и другими форматами файлов электронных таблиц.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Параметры ввода и загрузки |
| saveOptions | LowCodeSaveOptions | Параметры вывода и сохранения |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class JsonConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Создать пример данных JSON
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // Создайте поток памяти с данными JSON
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // Обработайте данные JSON с параметрами LowCode
                JsonConverter.Process(
                    new LowCodeLoadOptions() { InputStream = stream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.json"
                    });
            }

            Console.WriteLine("JSON processing completed successfully.");
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


