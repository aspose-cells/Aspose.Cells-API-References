---
title: "PivotAreaCollection.Add"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotAreaCollection 方法。添加透视区域"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareacollection/add/
---
## Add(PivotArea) {#add}

添加透视区域。

```csharp
[Obsolete("Use PivotAreaCollection.AddPivotArea(PivotArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(PivotArea pivotArea)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivotArea | PivotArea | 该透视区域。 |

### 备注

注意：此成员已过时。请改用 AddPivotArea() 方法。该方法将在自 2025 年 12 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionMethodAddWithPivotAreaDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("PivotTable");
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // 添加透视表
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // 向透视区域添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // 创建条件格式
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            // 创建透视区域并添加到集合
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            pcf.PivotAreas.Add(pivotArea);

            // 添加格式条件
            FormatCondition fc = pcf.FormatConditions[pcf.FormatConditions.AddCondition(FormatConditionType.CellValue)];
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Formula1 = "15";
            fc.Style.BackgroundColor = Color.Yellow;

            // 计算数据并保存
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotAreaCollectionMethodAddWithPivotAreaDemo_out.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

基于透视表视图添加区域。

```csharp
public void Add(CellArea cellArea)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | CellArea | 基于数据透视表视图的区域。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表创建示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // 添加数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // 定义要添加到数据透视表区域的单元格区域
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 0;
            cellArea.StartColumn = 0;
            cellArea.EndRow = 2;
            cellArea.EndColumn = 1;

            // 通过选择区域获取数据透视表区域集合
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea);

            try
            {
                // 使用 CellArea 参数调用 Add 方法
                pivotAreas.Add(cellArea);

                Console.WriteLine("Pivot area added successfully for cell area: " +
                    $"({cellArea.StartRow},{cellArea.StartColumn}) to ({cellArea.EndRow},{cellArea.EndColumn})");

                // 显示已添加的数据透视表区域
                foreach (PivotArea area in pivotAreas)
                {
                    CellArea[] areas = area.GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Pivot area covers: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("PivotAreaCollectionMethodAddWithCellAreaDemo.xlsx");
        }
    }
}
```

### 另请参见

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


