---
title: "PivotGlobalizationSettings.GetTextOfTotal"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取数据透视表中“总计”标签的文本。当数据透视表在数据区域包含两个或更多 PivotFields 时，需要重写此方法"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/
---
## PivotGlobalizationSettings.GetTextOfTotal method

获取 PivotTable 中 "Total" 标签的文本。当 PivotTable 在数据区域包含两个或更多 PivotField 时，需要重写此方法。

```csharp
public virtual string GetTextOfTotal()
```

### 返回值

"Total" 标签的文本

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfTotalDemo
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

            // 创建并使用全局化设置
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // 演示 GetTextOfTotal 方法
            Console.WriteLine("Total label text: " + globalizationSettings.GetTextOfTotal());

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


