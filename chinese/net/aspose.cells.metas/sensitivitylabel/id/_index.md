---
title: "SensitivityLabel.Id"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SensitivityLabel 属性。获取和设置敏感度标签的 id"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

获取和设置敏感度标签的 ID。

```csharp
public string Id { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIdDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 创建敏感度标签实例
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // 演示设置和获取 Id 属性
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // 显示 Id 值
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // 更改 Id 值以演示它是可读写的
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // 显示该属性影响其他操作
                label.IsEnabled = true;
                Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
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

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


