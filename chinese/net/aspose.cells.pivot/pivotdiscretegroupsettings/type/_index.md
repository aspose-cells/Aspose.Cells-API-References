---
title: "PivotDiscreteGroupSettings.Type"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotDiscreteGroupSettings 属性。获取分组类型"
type: docs
url: /zh/net/aspose.cells.pivot/pivotdiscretegroupsettings/type/
---
## PivotDiscreteGroupSettings.Type property

获取分组类型。

```csharp
public override PivotFieldGroupType Type { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDiscreteGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 示例数据
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 分组项
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { 
                new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }) 
            }, true);

            // 获取分组设置并演示 Type 属性
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);

            workbook.Save("PivotDiscreteGroupSettingsDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


