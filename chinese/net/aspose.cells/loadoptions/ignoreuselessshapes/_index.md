---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LoadOptions 属性。指示是否忽略无用的形状"
type: docs
url: /zh/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

指示是否忽略无用的形状。

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### 备注

仅适用于 xlsx、xlsb 和 xlsm 文件。某些文件中存在许多重叠的相同形状，这些形状是无用的，我们可以在加载文件时忽略它们。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // 创建加载选项并将 IgnoreUselessShapes 设置为 true
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // 使用这些选项加载工作簿
            Workbook workbook = new Workbook("example.xlsx", options);

            // 输出第一个工作表中形状的数量
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### 另请参见

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


