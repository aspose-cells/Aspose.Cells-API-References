---
title: "ConversionUtility.Convert"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ConversionUtility 方法。将 Excel 文件转换为其他格式"
type: docs
url: /zh/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

将 Excel 文件转换为其他格式。

```csharp
public static void Convert(string source, string saveAs)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 源 | String | 源文件名。 |
| saveAs | String | 预期文件的文件名。 |

### 示例

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
            // 初始化源文件和目标文件路径
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // 将 Excel 文件转换为 PDF
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### 另请参见

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

将 Excel 文件转换为其他格式。

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 源 | String | 源文件名。 |
| loadOptions | LoadOptions | 加载源文件的选项。 |
| saveAs | String | 预期文件的文件名。 |
| saveOptions | SaveOptions | 保存文件的选项。 |

### 示例

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
            // 源文件和目标文件路径
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // 创建示例 CSV 文件用于演示
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // 为 CSV 文件创建加载选项
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // 为 XLSX 文件创建保存选项
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // 使用指定选项将 CSV 转换为 XLSX
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // 通过加载输出文件验证转换
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // 清理临时文件
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### 另请参见

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


