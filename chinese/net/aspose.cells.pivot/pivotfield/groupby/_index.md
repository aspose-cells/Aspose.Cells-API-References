---
title: "PivotField.GroupBy"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。自动按间隔对字段进行分组"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

自动按间隔对字段进行分组

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 间隔 | Double | 组的内部。如果为零，将分配自动值， |
| newField | 布尔 | 指示是否向数据透视表添加新字段。仅适用于 DateTime 分组。 |

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 访问第一个数据透视表
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // 将字段添加到列区域
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // 按 1（间隔）对字段进行分组，使用自动范围
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

自动使用内部对字段进行分组

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 组 | PivotGroupByType[] | 分组类型 |
| 间隔 | Double | 组的内部。如果为零，将分配自动值，仅适用于按数字或天数分组。 |
| newField | 布尔 | 指示是否向数据透视表添加新字段。 |

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 另请参见

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

按日期分组类型对文件进行分组。

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 开始日期时间 |
| 结束 | DateTime | 结束日期时间 |
| 组 | PivotGroupByType[] | 分组类型 |
| 间隔 | Double | 间隔 |
| firstAsNewField | 布尔 | 指示是否向数据透视表添加新字段。仅适用于第一个分组项。 |

### 返回值

False 表示此字段无法按日期时间分组。

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加带日期的示例数据
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // 获取透视字段
            PivotField pivotField = pivotTable.RowFields[0];

            // 准备 GroupBy 方法的参数
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // 使用日期参数调用 GroupBy 方法
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // 刷新数据透视表
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

按日期分组类型对文件进行分组。

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAutoStart | 布尔 | 指示是否自动检测开始日期时间值。 |
| 开始 | DateTime | 开始日期时间 |
| isAutoEnd | 布尔 | 指示是否自动检测结束日期时间值。 |
| 结束 | DateTime | 结束日期时间 |
| 组 | PivotGroupByType[] | 分组类型 |
| 间隔 | Double | 间隔 |
| firstAsNewField | 布尔 | 指示是否向数据透视表添加新字段。仅适用于第一个分组项。 |

### 返回值

False 表示此字段无法按日期时间分组。

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 另请参见

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

按数字对文件进行分组。

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | Double | 开始值 |
| 结束 | Double | 结束值 |
| 间隔 | Double | 间隔 |
| newField | 布尔 | 指示是否向数据透视表添加新字段 |

### 返回值

False 表示此字段无法按日期时间分组。

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 添加行字段并对其进行分组
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // 保存工作簿
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

按数字对文件进行分组。

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAutoStart | 布尔 | 指示是否自动检测开始值。 |
| 开始 | Double | 开始值 |
| isAutoEnd | 布尔 | 指示是否自动检测结束值。 |
| 结束 | Double | 结束值 |
| 间隔 | Double | 间隔 |
| newField | 布尔 | 指示是否向数据透视表添加新字段 |

### 返回值

False 表示此字段无法按日期时间分组。

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions) 方法。该方法将在自 2026 年 9 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

自定义字段分组。

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | 自定义组项目。 |
| newField | 布尔 | 指示是否向数据透视表添加新字段 |

### 返回值

False 表示此字段无法按日期时间分组。

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions options) 方法，并使用 PivotFieldGroupOptions.DiscreteGroupItems 属性。此方法将在自 2026 年 7 月起的 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // 获取透视字段
            PivotField pivotField = pivotTable.RowFields[0];

            // 创建自定义组项目
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // 使用自定义组项目调用 GroupBy 方法
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // 刷新数据透视表
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

自定义字段分组。

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | 自定义组项目。 |
| newField | 布尔 | 指示是否向数据透视表添加新字段 |

### 备注

注意：此方法现已过时。请改用 PivotField.Group(PivotFieldGroupOptions options) 方法，并使用 PivotFieldGroupOptions.DiscreteGroupItems 属性。此方法将在自 2026 年 7 月起的 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 另请参见

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


