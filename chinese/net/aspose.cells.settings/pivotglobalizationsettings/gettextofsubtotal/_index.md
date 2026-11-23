---
title: "PivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取 PivotTable 中 PivotFieldSubtotalType 类型的文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/
---
## PivotGlobalizationSettings.GetTextOfSubTotal method

获取 PivotTable 中 [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) 类型的文本。

```csharp
public virtual string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | 此 [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### 返回值

给定类型的文本

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // 创建全局化设置
            Aspose.Cells.Settings.PivotGlobalizationSettings globalizationSettings = new Aspose.Cells.Settings.PivotGlobalizationSettings();

            // 演示使用不同小计类型的 GetTextOfSubTotal
            Console.WriteLine("Sum Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Sum));
            Console.WriteLine("Count Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Count));
            Console.WriteLine("Average Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Average));
            Console.WriteLine("Max Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Max));
            Console.WriteLine("Min Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Min));

            // 保存工作簿
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


