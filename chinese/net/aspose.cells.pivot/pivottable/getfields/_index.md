---
title: "PivotTable.GetFields"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 方法。按区域获取特定的透视字段列表"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/getfields/
---
## PivotTable.GetFields method

按区域获取特定的透视字段列表。

```csharp
public PivotFieldCollection GetFields(PivotFieldType fieldType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldType | PivotFieldType | 区域类型。 |

### 返回值

特定的透视字段集合

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodGetFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // 使用 PivotFieldType.Row 参数调用 GetFields 方法
                PivotFieldCollection rowFields = pivotTable.GetFields(PivotFieldType.Row);
                
                Console.WriteLine($"Number of row fields: {rowFields.Count}");
                foreach (PivotField field in rowFields)
                {
                    Console.WriteLine($"Row field name: {field.Name}");
                }

                // 使用 PivotFieldType.Data 参数调用 GetFields 方法
                PivotFieldCollection dataFields = pivotTable.GetFields(PivotFieldType.Data);
                
                Console.WriteLine($"Number of data fields: {dataFields.Count}");
                foreach (PivotField field in dataFields)
                {
                    Console.WriteLine($"Data field name: {field.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFields method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("PivotTableGetFieldsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


