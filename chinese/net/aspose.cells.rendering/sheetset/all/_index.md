---
title: "SheetSet.All"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SheetSet 属性。获取工作簿中所有工作表的集合，保持原始顺序"
type: docs
url: /zh/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

获取工作簿中所有工作表按原始顺序排列的集合。

```csharp
public static SheetSet All { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // 创建一个包含两个工作表的工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // 在两个工作表中设置一些示例数据
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // 将所有工作表保存为 markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### 另请参见

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


