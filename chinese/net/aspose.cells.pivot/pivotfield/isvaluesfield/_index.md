---
title: "PivotField.IsValuesField"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。指示此字段是否为值字段"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/isvaluesfield/
---
## PivotField.IsValuesField property

指示此字段是否为值字段。

```csharp
public bool IsValuesField { get; }
```

### 备注

仅在透视表视图中有两个或更多数据字段时有效。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValuesFieldDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";

            cells["A2"].Value = "Fruit";
            cells["B2"].Value = "Apple";
            cells["C2"].Value = 100;

            cells["A3"].Value = "Fruit";
            cells["B3"].Value = "Orange";
            cells["C3"].Value = 150;

            cells["A4"].Value = "Vegetable";
            cells["B4"].Value = "Carrot";
            cells["C4"].Value = 200;

            cells["A5"].Value = "Vegetable";
            cells["B5"].Value = "Potato";
            cells["C5"].Value = 250;

            // 添加透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // 获取数据字段（Sales）
                PivotField dataField = pivotTable.DataFields[0];

                // 显示 IsValuesField 属性值
                Console.WriteLine("IsValuesField value: " + dataField.IsValuesField);

                // 获取用于比较的行字段（Category）
                PivotField rowField = pivotTable.RowFields["Category"];
                Console.WriteLine("Row field IsValuesField value: " + rowField.IsValuesField);

                // 计算数据并刷新
                pivotTable.CalculateData();

                // 保存工作簿
                workbook.Save("IsValuesFieldDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


