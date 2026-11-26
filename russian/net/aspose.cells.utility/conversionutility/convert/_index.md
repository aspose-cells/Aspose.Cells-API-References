---
title: "ConversionUtility.Convert"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ConversionUtility. Преобразует файлы Excel в другие форматы"
type: docs
url: /ru/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Преобразует файлы Excel в другие форматы.

```csharp
public static void Convert(string source, string saveAs)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | String | Имя исходного файла. |
| saveAs | String | Имя ожидаемого файла. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ConversionUtilityMethodConvertWithStringStringDemo
    {
        public static void Run()
        {
            // Инициализировать пути к исходному и целевому файлам
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // Преобразовать файл Excel в PDF
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### См. также

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Преобразует файлы Excel в другие форматы.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | String | Имя исходного файла. |
| loadOptions | LoadOptions | Параметры загрузки исходного файла. |
| saveAs | String | Имя ожидаемого файла. |
| saveOptions | SaveOptions | Параметры сохранения файла. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
    {
        public static void Run()
        {
            // Пути к исходному и целевому файлам
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // Создать пример CSV‑файла для демонстрации
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // Создать параметры загрузки CSV‑файла
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // Создать параметры сохранения XLSX‑файла
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // Преобразовать CSV в XLSX с указанными параметрами
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // Проверить преобразование, загрузив выходной файл
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Очистите временные файлы
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### См. также

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


