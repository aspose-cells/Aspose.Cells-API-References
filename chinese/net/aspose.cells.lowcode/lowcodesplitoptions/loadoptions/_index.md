---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSplitOptions 属性。用于加载将被拆分的电子表格的加载选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

用于加载将要拆分的电子表格的加载选项。

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // 创建拆分选项实例
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // 初始化加载选项
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // 使用不同设置创建新的加载选项（使用可用属性）
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // 演示最终配置
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


