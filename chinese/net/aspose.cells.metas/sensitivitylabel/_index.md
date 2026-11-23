---
title: "类 SensitivityLabel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Metas.SensitivityLabel 类。表示敏感度标签"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

表示敏感度标签。

```csharp
public class SensitivityLabel
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | 获取和设置敏感度标签的分配方法。 |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | 获取和设置应应用于文件的内容标记类型。 |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | 获取和设置敏感度标签的 ID。 |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | 指示敏感度标签是否已启用 |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | 指示敏感度标签是否已被移除。 |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | 表示对应于描述敏感度标签的敏感度标签策略的 Azure Active Directory（Azure AD）站点标识符。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 使用反射创建 SensitivityLabel 类的实例
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // 设置基本属性
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // 显示属性值
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // 保存工作簿
                workbook.Save("SensitivityLabelDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


