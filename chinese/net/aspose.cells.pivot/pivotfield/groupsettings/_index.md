---
title: "PivotField.GroupSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。获取数据透视字段的分组设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

获取数据透视字段的分组设置。

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### 备注

如果此字段未分组，将返回 Null。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyGroupSettingsDemo
    {
        public static void Run()
        {
            // 从源 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 访问第一个数据透视表
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // 访问第二个基础字段（假设它存在）
            if (pivotTable.BaseFields.Count > 1)
            {
                PivotField pivotField = pivotTable.BaseFields[1];
                
                // 检查字段是否具有分组设置
                if (pivotField.GroupSettings != null)
                {
                    Console.WriteLine("Field has grouping enabled");
                    Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
                }
                else
                {
                    Console.WriteLine("Field has no grouping settings");
                }
                
                // 数值字段分组示例
                if (pivotField.GroupSettings == null && 
                    pivotField.PivotItems.Count > 0 && 
                    pivotField.PivotItems[0].Value is double)
                {
                    // 按数值范围分组（10 单位间隔）
                    pivotField.GroupBy(10.0, false);
                    Console.WriteLine("Field grouped by numeric range");
                }
            }
            
            // 保存已修改的工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


