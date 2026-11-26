---
title: "Класс ConversionUtility"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Utility.ConversionUtility класс. Представляет утилиту для преобразования файлов в другие форматы"
type: docs
url: /ru/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Представляет утилиту для преобразования файлов в другие форматы.

```csharp
public class ConversionUtility
```

## Методы

| Имя | Описание |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Преобразует файлы Excel в другие форматы. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Преобразует файлы Excel в другие форматы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;
    using System.IO;

    public class UtilityClassConversionUtilityDemo
    {
        public static void Run()
        {
            // Создайте пример CSV-файла для конвертации
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Создайте пример содержимого CSV
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Преобразуйте CSV в XLSX, используя статический метод конвертации
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Проверьте конвертацию, проверив наличие выходного файла
                if (File.Exists(outputFile))
                {
                    Console.WriteLine("Output file created successfully");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Очистите временные файлы
                if (File.Exists(sourceFile))
                {
                    File.Delete(sourceFile);
                }
                if (File.Exists(outputFile))
                {
                    File.Delete(outputFile);
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


