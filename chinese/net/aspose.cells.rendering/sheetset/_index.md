---
title: "类 SheetSet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.SheetSet 类。描述一组工作表"
type: docs
url: /zh/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

描述一组工作表。

```csharp
public class SheetSet
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | 基于精确的工作表索引创建工作表集。 |
| [SheetSet](sheetset/#constructor_1)(params string[]) | 基于精确的工作表名称创建工作表集。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | 获取包含工作簿活动工作表的集合。 |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | 获取工作簿中所有工作表按原始顺序排列的集合。 |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | 获取工作簿中可见工作表的集合，按原始顺序排列。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // 创建一个 PdfSaveOptions 对象
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // 将 SheetSet 属性设置为仅包含活动工作表
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // 将工作簿保存为 PDF 文件
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // 将 SheetSet 属性设置为包含所有可见工作表
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // 将工作簿保存为 PDF 文件
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // 将 SheetSet 属性设置为包含所有工作表
            pdfSaveOptions.SheetSet = SheetSet.All;

            // 将工作簿保存为 PDF 文件
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


