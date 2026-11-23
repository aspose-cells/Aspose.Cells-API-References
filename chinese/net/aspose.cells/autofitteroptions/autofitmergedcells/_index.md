---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AutoFitterOptions 属性。指示在行中单元格合并时是否自动适配行高。默认值为 false。"
type: docs
url: /zh/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

指示在行中单元格合并时是否自动适配行高。默认值为 false。

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### 备注

注意：此成员现已过时。请改用 AutoFitterOptions.AutoFitMergedCellsType 属性。此属性将在自 2018 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建示例数据并合并单元格
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // 创建 AutoFitterOptions 并设置 AutoFitMergedCells
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // 对合并单元格的行进行自动适配
            worksheet.AutoFitRows(options);

            // 保存工作簿
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### 另请参见

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


