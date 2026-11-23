---
title: "PivotField.ShowValuesAs"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。当使用 ShowDataAs 计算时，以不同的显示格式显示数据字段的值"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

当使用 ShowDataAs 计算时，以不同的显示格式显示数据字段的值。

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | 数据显示格式类型。 |
| baseField | Int32 | ShowDataAs 计算所依据的字段索引。 |
| baseItemPositionType | PivotItemPositionType | 基项的位置类型。 |
| baseItem | Int32 | ShowDataAs 计算所依据的基项索引。仅在 baseItemPositionType 为 custom 时有效。 |

### 备注

注意：此属性已过时。请改用 PivotField.ShowValuesAs(PivotShowValuesAsType,int,int) 方法。该方法将在自 2026 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // 创建数据透视表
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // 添加行字段
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // 添加列字段
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // 添加数据字段并配置 ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // 计算数据并保存
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

为此数据透视字段设置 "显示值为" 计算。

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | "显示值为" 计算的类型。 |
| baseField | Int32 | 用于计算的基字段索引。 |
| baseItem | Int32 | 用于计算的基项目索引。使用 [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) 表示前一个项目，使用 [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) 表示后一个项目；非负值表示特定透视项目的序数索引。 |

### 备注

仅适用于数据字段。

### 另请参见

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

为此数据字段配置 “显示值为” 计算。

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | “显示值为”的计算类型。 |
| baseField | String | 用于计算的基字段名称。 |
| baseItem | String | 常规透视项目的标题。还接受保留的文字关键字：`(previous)` 表示前一个项目，`(next)` 表示下一个项目。如果所选计算类型不需要基项目，请传入 `null`。 |

### 另请参见

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


