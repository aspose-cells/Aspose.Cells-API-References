---
title: "SheetSet.Visible"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SheetSet 属性。获取工作簿中可见工作表的集合，保持原始顺序"
type: docs
url: /zh/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

获取工作簿中可见工作表的集合，按原始顺序排列。

```csharp
public static SheetSet Visible { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // 创建一个包含两个工作表的新工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // 隐藏第二个工作表
            workbook.Worksheets[1].IsVisible = false;

            // 设置保存选项，仅导出可见工作表
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // 保存工作簿（仅导出可见工作表）
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### 另请参见

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


