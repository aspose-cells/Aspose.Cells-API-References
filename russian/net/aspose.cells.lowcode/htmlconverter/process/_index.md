---
title: "HtmlConverter.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод HtmlConverter. Преобразует указанный файл шаблона между html и другими форматами"
type: docs
url: /ru/net/aspose.cells.lowcode/htmlconverter/process/
---
## Process(string, string) {#process_1}

Преобразует указанный файл шаблона между HTML и другими форматами.

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
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class HtmlConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Создать временный файл HTML для конвертации
            string templateFile = CreateSampleHtmlFile();
            string resultFile = "HtmlConversionResult.xlsx";

            try
            {
                // Обработать файлы напрямую с помощью HtmlConverter
                HtmlConverter.Process(templateFile, resultFile);

                Console.WriteLine($"Successfully converted '{templateFile}' to '{resultFile}'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Очистите временный файл
                if (File.Exists(templateFile))
                {
                    File.Delete(templateFile);
                }
            }
        }

        private static string CreateSampleHtmlFile()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Conversion");
            
            string tempFile = Path.GetTempFileName() + ".html";
            workbook.Save(tempFile, SaveFormat.Html);
            return tempFile;
        }
    }
}
```

### См. также

* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Преобразует файл между HTML и другими форматами файлов электронных таблиц.

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
    public class HtmlConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Создать простой шаблон HTML в памяти
            string htmlContent = "<html><body><h1>Test Document</h1><p>This is a test HTML document.</p></body></html>";
            using (MemoryStream template = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(htmlContent)))
            {
                // Конвертировать в PDF, используя параметры LowCode
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.pdf",
                        SaveFormat = SaveFormat.Pdf
                    });

                // Сбросить позицию потока для следующей конвертации
                template.Position = 0;

                // Конвертировать в HTML, используя параметры LowCode
                HtmlConverter.Process(
                    new LowCodeLoadOptions() { InputStream = template },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.html",
                        SaveFormat = SaveFormat.Html
                    });
            }

            Console.WriteLine("Conversions completed successfully.");
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


