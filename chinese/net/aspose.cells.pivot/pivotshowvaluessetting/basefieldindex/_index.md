---
title: "PivotShowValuesSetting.BaseFieldIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotShowValuesSetting 属性。表示在使用 ShowDataAs 计算时的基字段"
type: docs
url: /zh/net/aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/
---
## PivotShowValuesSetting.BaseFieldIndex property

表示在使用 ShowDataAs 计算时的 ShowDataAs 计算的基字段。

```csharp
public int BaseFieldIndex { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingPropertyBaseFieldIndexDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            try
            {
                // 创建数据透视表
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // 向数据透视表添加字段
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // 获取数据字段及其显示值设置
                PivotField dataField = pivotTable.DataFields[0];
                PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

                // 设置计算类型以演示 BaseFieldIndex 的用法
                showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;

                // 设置和获取 BaseFieldIndex 属性
                showValuesSetting.BaseFieldIndex = 0;
                Console.WriteLine("BaseFieldIndex value: " + showValuesSetting.BaseFieldIndex);

                // 刷新并计算数据透视表
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // 保存工作簿
                workbook.Save("BaseFieldIndexDemo.xlsx");
                Console.WriteLine("BaseFieldIndex has been demonstrated successfully.");
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

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


