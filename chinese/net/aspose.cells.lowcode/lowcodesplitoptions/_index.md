---
title: "类 LowCodeSplitOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeSplitOptions 类。用于拆分电子表格的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

拆分电子表格的选项。

```csharp
public class LowCodeSplitOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | 用于加载将要拆分的电子表格的加载选项。 |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | 用于保存拆分后部分的保存选项。 |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | 提供用于保存拆分后部分的保存选项的提供程序。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 使用示例数据填充工作表
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // 创建 LowCodeSplitOptions 的实例
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // 配置 LoadOptions（示例：处理受密码保护的源）
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // 配置 SaveOptions（示例：设置默认输出格式）
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // 实现用于动态输出设置的自定义 SaveOptions 提供程序
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // 示例集成：使用已配置的选项将工作簿拆分为多个部分
            // (假设存在类似 LowCodeEngine.Split(workbook, splitOptions, \"outputDir\") 的方法)
            // LowCodeEngine.Split(workbook, splitOptions, \"OutputDirectory\");
            
            // 保存原始工作簿以作演示
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // 自定义 SaveOptionsProvider 实现
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // 示例逻辑：基于拆分索引的备用设置
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


