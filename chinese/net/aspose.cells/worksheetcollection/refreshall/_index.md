---
title: "WorksheetCollection.RefreshAll"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorksheetCollection 方法。使用数据透视源刷新所有数据透视表和图表"
type: docs
url: /zh/net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

使用数据透视源刷新所有数据透视表和图表。

```csharp
[Obsolete("Use Workbook.RefreshAll() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RefreshAll()
```

### 备注

注意：此成员已过时。请改用 Workbook.RefreshAll() 方法。该方法将在自 2026 年 4 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshAllDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据和公式
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            
            // 添加将被刷新的公式
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["C2"].PutValue("=SUM(B2:B3)");
            
            // 更改一些值
            worksheet.Cells["B2"].PutValue(3.0);
            worksheet.Cells["B3"].PutValue(2.0);
            
            // 刷新所有工作表中的所有公式
            workbook.Worksheets.RefreshAll();
            
            // 输出已刷新总计
            Console.WriteLine("Refreshed total: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### 另请参见

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


