---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptionsProviderOfAssembling 属性。是否始终将工作表索引或名称添加到文件路径。默认值为 false，即当只有一个工作表时，工作表索引或名称以及相应的前缀不会添加到文件路径中。"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property

是否始终在文件路径中添加工作表索引或名称。默认值为 false，即当只有一个工作表时，工作表索引（或名称）及相应前缀不会添加到文件路径中。

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // 创建一个仅包含一个工作表的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // 创建 LowCodeSaveOptionsProviderOfAssembling 的实例
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            
            // 配置路径设置
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = true; // Use sheet name instead of index
            provider.SheetPrefix = "_Sheet_";
            provider.SplitPartPrefix = "_Part_";
            
            // 显示初始属性值
            Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
            
            // 演示未使用 BuildPathWithSheetAlways 的文件路径
            string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (default): " + defaultPath);
            
            // 将 BuildPathWithSheetAlways 设置为 true
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
            
            // 演示使用 BuildPathWithSheetAlways 的文件路径（即使只有单个工作表）
            string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (updated): " + updatedPath);
            
            // 保存工作簿（在实际场景中，拆分行为将使用提供程序的设置）
            workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


