---
title: "枚举 SignificantDigitsType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.SignificantDigitsType 枚举。表示用于输出数值的有效数字类型"
type: docs
url: /zh/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

表示用于输出数值的有效数字类型。

```csharp
public enum SignificantDigitsType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Digits15 | `0` | 15 位数字 |
| G17 | `1` | 通过使用 "G17" 格式化值来实现 17 位数字。 |
| Rounding17 | `2` | 通过对值进行四舍五入实现 17 位数字。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个用于演示的新工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 演示使用每个 SignificantDigitsType 枚举值
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // 为工作簿设置有效数字类型
                    workbook.Settings.SignificantDigitsType = type;

                    // 显示当前设置
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // 添加示例值以演示该设置
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // 使用当前设置保存工作簿
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


