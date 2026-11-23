---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DeleteBlankOptions 属性。指示是否将绘图相关对象（如图片、形状、图表...）视为空白。默认值为 true"
type: docs
url: /zh/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

指示是否将图片、形状、图表等绘图相关对象视为空白。默认值为 true。

```csharp
public bool DrawingsAsBlank { get; set; }
```

### 备注

当将此属性设置为 false 时，所有被绘图对象覆盖的行/列将不被视为空白，也不会被删除。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // 添加一个绘图对象以测试 DrawingsAsBlank 行为
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // 在 DrawingsAsBlank = false 时删除空白列（保留绘图）
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### 另请参见

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


