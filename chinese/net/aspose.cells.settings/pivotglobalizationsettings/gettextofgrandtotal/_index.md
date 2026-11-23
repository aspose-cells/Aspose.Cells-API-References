---
title: "PivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取 PivotTable 中 Grand Total 标签的文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofgrandtotal/
---
## PivotGlobalizationSettings.GetTextOfGrandTotal method

获取 PivotTable 中 "Grand Total" 标签的文本。

```csharp
public virtual string GetTextOfGrandTotal()
```

### 返回值

“Grand Total” 标签的文本

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 创建全局化设置并演示 GetTextOfGrandTotal
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Grand Total Text: " + globalizationSettings.GetTextOfGrandTotal());

            // 保存工作簿
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


