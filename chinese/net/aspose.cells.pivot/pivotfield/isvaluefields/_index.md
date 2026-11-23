---
title: "PivotField.IsValueFields"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。指示此字段是否表示值字段"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/isvaluefields/
---
## PivotField.IsValueFields property

指示此字段是否表示值字段。

```csharp
[Obsolete("Use PivotField.IsValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsValueFields { get; }
```

### 备注

注意：此方法已过时。请改用 PivotField.IsValuesField 属性。此方法将在自2023年11月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValueFieldsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["A5"].Value = "Car";
            worksheet.Cells["B2"].Value = "East";
            worksheet.Cells["B3"].Value = "West";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["B5"].Value = "West";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 3000;
            worksheet.Cells["C5"].Value = 4000;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // 添加列字段
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");

            // 添加数据字段并从 DataFields 集合中获取它
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];

            // 显示 IsValueFields 属性值
            Console.WriteLine("IsValueFields for data field: " + dataField.IsValueFields);

            // 尝试查找非数据字段以显示 IsValueFields 为 false
            foreach (PivotField field in pivotTable.RowFields)
            {
                Console.WriteLine("IsValueFields for row field '" + field.Name + "': " + field.IsValueFields);
            }

            // 保存结果
            workbook.Save("PivotFieldPropertyIsValueFieldsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


