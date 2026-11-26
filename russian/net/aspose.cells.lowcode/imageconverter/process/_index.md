---
title: "ImageConverter.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ImageConverter. Преобразует файл шаблона в изображения"
type: docs
url: /ru/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Преобразует файл шаблона в изображения.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | String | Файл шаблона, который будет преобразован в изображения. |
| resultFile | String | Полученный файл (шаблон имени) для сгенерированных изображений. |

### Примечания

Файлы вывода будут созданы из указанного результирующего файла путем добавления номера последовательности листа и части разделения. Например, если указанный файл вывода — Image.png, то сгенерированные файлы изображений будут Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую рабочую книгу и заполнить её примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // Сохранить как файл шаблона для обработки
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // Преобразовать шаблон в изображения, используя параметры (String, String)
                ImageConverter.Process("Template.xlsx", "OutputSheet.png");

                Console.WriteLine("Process method executed successfully. Generated image(s) from spreadsheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image conversion: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Преобразует файл шаблона в изображения

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Параметры ввода и загрузки |
| saveOptions | LowCodeSaveOptions | Параметры вывода и сохранения |

### Примечания

При конвертации в изображение формата, поддерживающего несколько страниц (например, tiff), указанные [`OutputFile`](../../lowcodesaveoptions/outputfile/) или [`OutputStream`](../../lowcodesaveoptions/outputstream/) будут использованы напрямую для результирующего изображения. Для других типов изображений, если параметры сохранения указали Stream в качестве вывода, все результирующие изображения будут сохранены в один и тот же Stream. В противном случае файлы вывода будут созданы из указанного файла вывода параметров сохранения путем добавления номера последовательности листа и части разделения. Например, если указанный файл вывода — Image.png, то сгенерированные файлы изображений будут Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            try
            {
                // Инициализировать LowCodeLoadOptions с файлом шаблона
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // Инициализировать LowCodeSaveOptions с каталогом вывода
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // Выполнить метод Process с указанными параметрами
                ImageConverter.Process(loadOptions, saveOptions);
                
                Console.WriteLine("Spreadsheet converted to images successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during processing: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Преобразует файл шаблона в изображения

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Параметры ввода и загрузки |
| saveOptions | LowCodeSaveOptions | Параметры сохранения. Его вывод ([`OutputFile`](../../lowcodesaveoptions/outputfile/) или [`OutputStream`](../../lowcodesaveoptions/outputstream/)) не оказывает влияния, поскольку все выводы будут указаны параметром "provider". |
| провайдер | AbstractLowCodeSaveOptionsProvider | Провайдер параметров сохранения для сохранения сгенерированных изображений |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
            const string templatePath = "SampleTemplate.xlsx";
            const string outputDir = "Output/";
            
            // Создать примерный шаблон
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // Инициализировать параметры загрузки
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // Настроить параметры сохранения с использованием LowCodeImageSaveOptions
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // Вызвать статический метод Process
                ImageConverter.Process(loadOptions, saveOptions, provider);
                Console.WriteLine($"Generated PNG images in: {Path.GetFullPath(outputDir)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Processing failed: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string path)
        {
            using (Workbook wb = new Workbook())
            {
                Worksheet sheet = wb.Worksheets[0];
                sheet.Cells["A1"].PutValue("LowCode Process Demo");
                sheet.Cells["B3"].PutValue(DateTime.Now.ToString());
                wb.Save(path, SaveFormat.Xlsx);
            }
        }

        private class DynamicSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            private readonly LowCodeImageSaveOptions _baseOptions; // Corrected type

            public DynamicSaveOptionsProvider(LowCodeImageSaveOptions options)
            {
                _baseOptions = options;
            }

            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Получить свойства разрешения из LowCodeImageSaveOptions
                if (partInfo.SheetIndex == 0)
                {
                    _baseOptions.ImageOptions.HorizontalResolution = 300;
                    _baseOptions.ImageOptions.VerticalResolution = 300;
                }
                return _baseOptions;
            }
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


