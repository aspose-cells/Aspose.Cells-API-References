---
title: "类 ConversionUtility"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Utility.ConversionUtility 类。表示用于将文件转换为其他格式的实用程序"
type: docs
url: /zh/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

表示用于将文件转换为其他格式的实用程序。

```csharp
public class ConversionUtility
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | 将 Excel 文件转换为其他格式。 |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | 将 Excel 文件转换为其他格式。 |

### 示例

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
            // 创建用于转换的示例 CSV 文件
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // 创建示例 CSV 内容
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // 使用静态转换方法将 CSV 转换为 XLSX
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // 通过检查输出文件是否存在来验证转换
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
                // 清理临时文件
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

### 另请参见

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


