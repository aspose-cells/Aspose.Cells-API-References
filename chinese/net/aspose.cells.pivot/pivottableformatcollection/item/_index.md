---
title: "PivotTableFormatCollection.Item"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTableFormatCollection 属性。通过索引获取格式"
type: docs
url: /zh/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

按索引获取格式。

```csharp
public PivotTableFormat this[int index] { get; }
```

| 参数 | 描述 |
| --- | --- |
| 索引 | 索引。 |

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");

            // 刷新所有数据透视表
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // 访问第一个数据透视表
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // 通过访问第一个 PivotFormat 演示 Item 属性
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // 使用 Item 属性更改格式设置
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // 保存已修改的工作簿
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


