---
title: "类 LowCodeMergeOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeMergeOptions 类。将多个模板文件合并为一个的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

将多个模板文件合并为一个的选项。

```csharp
public class LowCodeMergeOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | 提供用于保存拆分后部分的保存选项的提供程序。 |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | 用于保存拆分后部分的保存选项。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 创建并配置 LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // 设置输出格式的保存选项
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // 分配自定义加载选项提供程序
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // 示例集成（带合并功能的假设用法）
            // 这通常会使用实际的文件路径调用
            // Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
            
            // 保存工作簿（演示目的）
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // 实现抽象类的自定义提供程序
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // 满足抽象要求的最小实现
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


