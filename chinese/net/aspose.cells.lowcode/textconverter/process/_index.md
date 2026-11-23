---
title: "TextConverter.Process"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextConverter 方法。将给定的模板文件在基于文本的文件和其他格式之间转换"
type: docs
url: /zh/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

在基于文本的文件与其他格式之间转换给定的模板文件。

```csharp
public static void Process(string templateFile, string resultFile)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | String | 待转换的模板文件 |
| resultFile | String | 生成的文件 |

### 示例

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

            // 创建示例 CSV 文件
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // 直接调用静态 Process 方法，无需实例化 TextConverter
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
                // 清理临时文件
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### 另请参见

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

在基于文本的格式与其他电子表格文件格式之间转换文件格式

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | 输入和加载的选项 |
| saveOptions | LowCodeSaveOptions | 输出和保存的选项 |

### 示例

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
            // 创建示例文本文件
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // 使用 LowCode 选项处理文本文件
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

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


