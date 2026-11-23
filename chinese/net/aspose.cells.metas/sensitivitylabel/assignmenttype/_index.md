---
title: "SensitivityLabel.AssignmentType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SensitivityLabel 属性。获取和设置敏感度标签的分配方法"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

获取和设置敏感度标签的分配方法。

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyAssignmentTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 创建敏感度标签实例
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // 设置基本属性
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // 演示获取初始 AssignmentType 值
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // 将 AssignmentType 设置为 Privileged 并显示更改
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // 改回 Standard 以演示其可读写
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // 保存工作簿
                workbook.Save("AssignmentTypeDemo.xlsx");
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

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


