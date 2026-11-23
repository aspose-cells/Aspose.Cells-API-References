---
title: "SheetSet.Active"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SheetSet 属性。获取工作簿中活动工作表的集合"
type: docs
url: /zh/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

获取包含工作簿活动工作表的集合。

```csharp
public static SheetSet Active { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // 创建一个包含两个工作表的新工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // 将第二个工作表设为活动状态
            workbook.Worksheets.ActiveSheetIndex = 1;

            // 向两个工作表添加数据
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // 创建 PDF 保存选项
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // 仅保存活动工作表
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // 保存所有工作表以进行比较
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### 另请参见

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


