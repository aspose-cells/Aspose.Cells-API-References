---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSplitOptions 属性。用于保存拆分部件的保存选项提供程序"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

提供用于保存拆分后部分的保存选项的提供程序。

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### 备注

如果指定了此属性，[`SaveOptions`](../saveoptions/) 将不生效，因为每个拆分部件的输出将由提供程序指定。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 填充一些示例数据
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // 创建 LowCodeSplitOptions 实例
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // 显示当前 SaveOptionsProvider 值（默认 null）
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // 创建自定义 SaveOptionsProvider
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // 演示设置 SaveOptionsProvider 的效果
            // 在实际场景中，这将在拆分文件时使用
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // 保存工作簿（尽管此处未演示拆分）
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // AbstractLowCodeSaveOptionsProvider 的自定义实现
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // 为每个拆分部件创建自定义保存选项
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // 在保存每个部件后执行任何清理工作
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### 另请参见

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


