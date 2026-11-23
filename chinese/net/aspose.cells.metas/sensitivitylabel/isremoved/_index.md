---
title: "SensitivityLabel.IsRemoved"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SensitivityLabel 属性。指示是否已删除敏感度标签"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

指示敏感度标签是否已被移除。

```csharp
public bool IsRemoved { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsRemovedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 通过反射创建敏感度标签实例
                // 因为无法直接实例化
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // 设置必需的属性
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // 显示初始 IsRemoved 值
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // 演示设置 IsRemoved 属性（因为它是可读写的）
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // 切换该值以显示它可以被更改
                label.IsRemoved = false;
                Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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


