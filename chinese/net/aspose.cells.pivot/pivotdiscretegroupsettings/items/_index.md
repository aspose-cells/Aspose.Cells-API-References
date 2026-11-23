---
title: "PivotDiscreteGroupSettings.Items"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotDiscreteGroupSettings 属性。获取离散项"
type: docs
url: /zh/net/aspose.cells.pivot/pivotdiscretegroupsettings/items/
---
## PivotDiscreteGroupSettings.Items property

获取离散项。

```csharp
[Obsolete("Use PivotField.GroupBy(DiscreteGroupItem[], bool) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomPiovtFieldGroupItem[] Items { get; }
```

### 备注

注意：此方法现已过时。请改用 PivotField.GroupBy(DiscreteGroupItem[], bool) 方法。该方法将在自 2026 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsPropertyItemsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Apple");
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(150);
            worksheet.Cells["B6"].PutValue(250);

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // 获取透视字段并对其分组
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[0], false);

            // 访问离散分组设置
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // 显示当前项
            Console.WriteLine("Current Items count: " + groupSettings.Items.Length);
            foreach (CustomPiovtFieldGroupItem item in groupSettings.Items)
            {
                Console.WriteLine("Item: " + item.ToString());
            }

            // 保存工作簿
            workbook.Save("PivotDiscreteGroupSettingsItemsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


