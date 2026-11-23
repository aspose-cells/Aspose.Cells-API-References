---
title: "PivotField.NonAutoSortDefault"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。指示将应用于此透视字段的排序操作是自动排序还是普通数据排序"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

指示将应用于此透视字段的排序操作是自动排序还是普通数据排序。

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### 备注

注意：此属性现已过时。请改用 !PivotField.SortSetting.IsSimpleSort 属性。此方法将在自2026年9月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 访问第一个工作表和数据透视表
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // 访问数据透视表中的第一行字段
            PivotField pivotField = pivotTable.RowFields[0];
            
            // 将 NonAutoSortDefault 属性设置为 true
            pivotField.NonAutoSortDefault = true;
            
            // 输出属性值
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // 保存工作簿
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


