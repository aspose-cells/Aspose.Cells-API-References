---
title: "HtmlSaveOptions.SheetSet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置要呈现的工作表。默认是工作簿中所有可见的工作表 Visible"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

获取或设置要呈现的工作表。默认是工作簿中所有可见的工作表：[`Visible`](../../../aspose.cells.rendering/sheetset/visible/)。

```csharp
public SheetSet SheetSet { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // 创建一个包含多个工作表的新工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // 将一个工作表隐藏以作演示
            workbook.Worksheets[1].IsVisible = false;

            // 在每个工作表中设置一些示例数据
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // 创建 HtmlSaveOptions 实例
            HtmlSaveOptions options = new HtmlSaveOptions();

            // 显示当前 SheetSet 值（默认是 null，表示所有可见工作表）
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // 将 SheetSet 设置为仅包含特定工作表（按索引）
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // 保存为 HTML - 仅包含指定的工作表
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // 将 SheetSet 更改为仅可见工作表
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // 将 SheetSet 更改为仅活动工作表
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### 另请参见

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


