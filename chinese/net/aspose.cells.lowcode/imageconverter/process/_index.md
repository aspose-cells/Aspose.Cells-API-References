---
title: "ImageConverter.Process"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImageConverter 方法。将模板文件转换为图像"
type: docs
url: /zh/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

将模板文件转换为图像。

```csharp
public static void Process(string templateFile, string resultFile)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | String | 要转换为图像的模板文件。 |
| resultFile | String | 生成图像的结果文件（名称模式）。 |

### 备注

输出文件将基于指定的结果文件，通过附加工作表的序号和拆分部分来构建。例如，如果指定的输出文件为 Image.png，则生成的图像文件将是 Image_0_0.png、Image_0_1.png、...、Image_1_0.png、...

### 示例

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
            // 创建一个新的工作簿并填充示例数据
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // 保存为用于处理的模板文件
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // 使用 (String, String) 参数将模板转换为图像
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

### 另请参见

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

将模板文件转换为图像

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | 输入和加载的选项 |
| saveOptions | LowCodeSaveOptions | 输出和保存的选项 |

### 备注

在将支持多页的图像格式（例如 tiff）转换为图像时，指定的 [`OutputFile`](../../lowcodesaveoptions/outputfile/) 或 [`OutputStream`](../../lowcodesaveoptions/outputstream/) 将直接用于生成的图像。对于其他类型的图像，如果保存选项已将 Stream 指定为输出，则所有生成的图像将保存到同一 Stream。否则，输出文件将基于保存选项中指定的输出文件，通过附加工作表的序号和拆分部分来构建。例如，如果指定的输出文件为 Image.png，则生成的图像文件将是 Image_0_0.png、Image_0_1.png、...、Image_1_0.png、...

### 示例

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
                // 使用模板文件初始化 LowCodeLoadOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // 使用输出目录初始化 LowCodeSaveOptions
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // 使用指定参数执行 Process 方法
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

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

将模板文件转换为图像

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | 输入和加载的选项 |
| saveOptions | LowCodeSaveOptions | 保存选项。其输出（[`OutputFile`](../../lowcodesaveoptions/outputfile/) 或 [`OutputStream`](../../lowcodesaveoptions/outputstream/)）无效，因为所有输出将由 "provider" 参数指定 |
| provider | AbstractLowCodeSaveOptionsProvider | 用于保存生成图像的保存选项的提供者 |

### 示例

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
            
            // 创建示例模板
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // 初始化加载选项
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // 使用 LowCodeImageSaveOptions 配置保存选项
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // 调用静态 Process 方法
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
                // 从 LowCodeImageSaveOptions 访问分辨率属性
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

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


