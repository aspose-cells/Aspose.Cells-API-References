---
title: "Worksheet.GridlineColor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Worksheet 属性。获取和设置网格线的颜色"
type: docs
url: /zh/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

获取和设置网格线的颜色

```csharp
public Color GridlineColor { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 将网格线颜色设置为红色
            worksheet.GridlineColor = Color.Red;
            
            // 保存工作簿
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### 另请参见

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


