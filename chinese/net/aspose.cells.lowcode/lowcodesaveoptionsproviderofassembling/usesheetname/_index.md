---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptionsProviderOfAssembling 属性。是否使用工作表名称而不是工作表索引构建文件路径。默认值为 false"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

是否使用工作表名称而非工作表索引构建文件路径。默认值为 false。

```csharp
public bool UseSheetName { get; set; }
```

### 备注

工作表名称永远不会自动重新构建。因此当将其设置为 true 时，请确保没有可能导致文件路径或名称无效的特殊工作表名称。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // 创建带有命名工作表的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // 添加用于拆分演示的示例数据
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // 创建并配置提供程序
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // 演示 UseSheetName=false（默认）
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // 更改属性并演示新行为
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


