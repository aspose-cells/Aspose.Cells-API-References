---
title: "PdfConverter.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PdfConverter. Преобразует указанный файл шаблона в pdf"
type: docs
url: /ru/net/aspose.cells.lowcode/pdfconverter/process/
---
## Process(string, string) {#process_1}

Преобразует указанный файл шаблона в PDF.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | String | Файл шаблона для преобразования |
| resultFile | String | Полученный файл должен быть pdf-файлом. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class PdfConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Создать пример файла шаблона
            CreateSampleTemplate("template.xlsx");

            try
            {
                // Вызвать метод Process с параметрами (String, String) непосредственно на типе
                PdfConverter.Process("template.xlsx", "output.pdf");
                
                Console.WriteLine("Successfully converted template.xlsx to output.pdf");
                Console.WriteLine($"PDF created at: {Path.GetFullPath("output.pdf")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateSampleTemplate(string fileName)
        {
            using (Workbook workbook = new Workbook())
            {
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("PDF Conversion Test");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
                workbook.Save(fileName);
            }
        }
    }
}
```

### См. также

* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Преобразует файл шаблона в PDF

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
    public class PdfConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Создать пример входного потока (Excel‑файл в памяти)
            var workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Content");
            MemoryStream template = new MemoryStream();
            workbook.Save(template, SaveFormat.Xlsx);
            template.Position = 0;

            // Каталог вывода.
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Пример 1: Преобразовать в PDF
            Aspose.Cells.LowCode.PdfConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodePdfSaveOptions() 
                { 
                    OutputFile = outputDir + "output.pdf",
                    PdfOptions = new PdfSaveOptions()
                });

            // Пример 2: Преобразовать в HTML
            Aspose.Cells.LowCode.HtmlConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodeSaveOptions() 
                { 
                    OutputFile = outputDir + "output.html" 
                });

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


