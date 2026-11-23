---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。实现此接口以在渲染时获取 DrawObject 和 Bound"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

实现此接口以在渲染时获取 DrawObject 和 Bound。

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
    {
        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
            }
        }

        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加一些示例数据和形状
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // 创建一个 PaginatedSaveOptions 实例
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // 显示属性的当前值（初始应为 null）
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // 设置一个新的自定义事件处理程序
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // 这将在渲染期间触发 Draw 方法
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // 将事件处理程序更改为 null 以演示差异
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### 另请参见

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


