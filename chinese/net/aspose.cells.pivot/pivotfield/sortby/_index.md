---
title: "PivotField.SortBy"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。对该数据透视字段进行排序"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

对该数据透视字段进行排序。

```csharp
public void SortBy(SortOrder sortType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | SortOrder | 此字段的排序类型。 |

### 另请参见

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

对该数据透视字段进行排序。

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | SortOrder | 此字段的排序类型。 |
| fieldSortedBy | Int32 | 用于排序的透视字段索引。-1 表示按此字段的数据标签排序，其他值表示按数据字段的索引排序。 |

### 备注

注意：此属性已过时。请改用 PivotField.SortBy(SortOrder, int,string) 方法或 PivotField.IsAutoSort 属性。此方法将在自 2026 年 9 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 添加行字段
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // 使用索引 -1 将行字段按降序排序
            rowField.SortBy(SortOrder.Descending, -1);
            
            // 刷新并计算数据透视表
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // 保存工作簿
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

对该数据透视字段进行排序。

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | SortOrder | 此字段的排序类型。 |
| fieldSortedBy | Int32 | 用于排序的透视字段索引。-1 表示按此字段的数据标签排序，其他值表示按数据字段的索引排序。 |
| dataType | PivotLineType | 排序的数据类型。 |
| cellName | String | 按行或列的值排序 |

### 备注

注意：此属性已过时。请改用 PivotField.SortBy(SortOrder, int,string) 方法。此方法将在自 2026 年 9 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // 对行字段进行排序
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // 计算数据
            pivotTable.CalculateData();
            
            // 保存工作簿
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

对该数据透视字段进行排序。

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sortType | SortOrder | 此字段的排序类型。 |
| fieldSortedBy | Int32 | 用于排序的透视字段索引。-1 表示按此字段的数据标签排序，其他值表示按数据字段的索引排序。 |
| cellName | String | 按行或列的值排序。如果为 Null，则按字段的总计分组；否则按所选列或行的值分组。 |

### 另请参见

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


