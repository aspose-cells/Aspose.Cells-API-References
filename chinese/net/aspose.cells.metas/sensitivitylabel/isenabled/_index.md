---
title: "SensitivityLabel.IsEnabled"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SensitivityLabel 属性。指示敏感度标签是否已启用"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

指示敏感度标签是否已启用

```csharp
public bool IsEnabled { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsEnabledDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 创建敏感度标签实例
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // 设置初始属性
                label.Id = "CONFIDENTIAL_001";
                
                // 演示获取初始 IsEnabled 值
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // 将 IsEnabled 设置为 true 并显示更改
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // 切换该值以演示它是可读写的
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // 保存工作簿
                workbook.Save("IsEnabledDemo.xlsx");
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


