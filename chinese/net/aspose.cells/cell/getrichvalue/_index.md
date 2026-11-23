---
title: "Cell.GetRichValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 方法。获取单元格的富文本值"
type: docs
url: /zh/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

获取单元格的富文本值。

```csharp
public CellRichValue GetRichValue()
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook wb = new Workbook();
            
            // 访问第一个工作表
            Worksheet ws = wb.Worksheets[0];
            
            // 在单元格 A1 中设置富文本值
            ws.Cells["A1"].PutValue("This is rich text");
            
            // 从单元格 A1 获取富值
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // 显示富文本值
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // 保存工作簿
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


