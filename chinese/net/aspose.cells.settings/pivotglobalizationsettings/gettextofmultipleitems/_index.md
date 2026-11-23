---
title: "PivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取 PivotTable 中 Multiple Items 标签的文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/
---
## PivotGlobalizationSettings.GetTextOfMultipleItems method

获取 PivotTable 中 "(Multiple Items)" 标签的文本。

```csharp
public virtual string GetTextOfMultipleItems()
```

### 返回值

“(Multiple Items)” 标签的文本

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 创建并使用全局化设置
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // 演示 GetTextOfMultipleItems 以及其他关键方法
            Console.WriteLine("Multiple Items Text: " + settings.GetTextOfMultipleItems());
            Console.WriteLine("Total Text: " + settings.GetTextOfTotal());
            Console.WriteLine("Grand Total Text: " + settings.GetTextOfGrandTotal());

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


