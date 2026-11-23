---
title: "FontConfigs.IsFontAvailable"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FontConfigs 方法。指示字体是否可用"
type: docs
url: /zh/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

指示字体是否可用。

```csharp
public static bool IsFontAvailable(string fontName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontName | String | 字体名称 |

### 返回值

如果字体可用则为 true，否则为 false。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 测试字体名称以检查可用性
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // 使用字体名称调用 IsFontAvailable 方法
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // 显示结果
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // 将结果写入工作表
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


