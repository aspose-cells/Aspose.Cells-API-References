---
title: "AutoFitterOptions.ForRendering"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AutoFitterOptions 属性。指示是否适用于渲染目的"
type: docs
url: /zh/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

指示是否适用于渲染目的。

```csharp
public bool ForRendering { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 设置包含长文本的示例数据
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // 创建 AutoFitterOptions 并将 ForRendering 设置为 true
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // 在渲染考虑下自动调整行高
            worksheet.AutoFitRows(0, 0, options);

            // 输出结果行高（像素）
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### 另请参见

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


