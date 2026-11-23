---
title: "Metered.IsMeteredLicensed"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Metered 方法。检查是否已获得计量授权"
type: docs
url: /zh/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

检查是否已获得计量授权

```csharp
public static bool IsMeteredLicensed()
```

### 返回值

真或假

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 Metered 实例
            Metered metered = new Metered();

            try
            {
                // 检查是否已应用计量许可证
                bool isLicensed = Metered.IsMeteredLicensed();

                // 显示结果
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // 将结果添加到工作表中
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


