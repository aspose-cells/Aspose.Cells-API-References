---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DifLoadOptions 构造函数。选项"
type: docs
url: /zh/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

这些选项。

```csharp
public DifLoadOptions()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // 使用无参数构造函数创建 DifLoadOptions 的新实例
                DifLoadOptions loadOptions = new DifLoadOptions();

                // 使用默认选项创建新工作簿
                Workbook workbook = new Workbook();

                // 访问第一个工作表
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加示例数据以演示工作簿的功能
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // 以 DIF 格式保存工作簿
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // 现在使用 DifLoadOptions 加载已保存的 DIF 文件
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // 将加载的数据保存为 XLSX 以进行验证
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


