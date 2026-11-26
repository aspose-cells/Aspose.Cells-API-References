---
title: "TextConverter.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TextConverter. Преобразует указанный файл шаблона между текстовыми файлами и другими форматами"
type: docs
url: /ru/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

Преобразует указанный файл шаблона между текстовыми файлами и другими форматами.

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

    public class TextConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            string inputFile = "input.csv";
            string outputFile = "output.xlsx";

            // Создаёт примерный CSV‑файл
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // Вызовите статический метод Process напрямую без создания экземпляра TextConverter
                TextConverter.Process(inputFile, outputFile);
                
                Console.WriteLine($"Process method successfully converted {inputFile} to {outputFile}");
                Console.WriteLine($"Converted file exists: {File.Exists(outputFile)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            finally
            {
                // Очистите временные файлы
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### См. также

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Преобразует формат файла между текстовыми форматами и другими форматами файлов электронных таблиц

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
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Создайте пример текстового файла
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // Обработайте текстовый файл с параметрами LowCode
            using (FileStream inputStream = new FileStream(inputPath, FileMode.Open))
            {
                TextConverter.Process(
                    new LowCodeLoadOptions() { InputStream = inputStream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.txt"
                    }
                );
            }

            Console.WriteLine("Text processing completed successfully.");
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


