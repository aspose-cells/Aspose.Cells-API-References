---
title: "SensitivityLabel.ContentMarkType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SensitivityLabel 属性。获取和设置应应用于文件的内容标记类型"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

获取和设置应应用于文件的内容标记类型。

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyContentMarkTypeDemo
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
                
                // 演示 ContentMarkType 属性（读写）
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // 设置不同的内容标记类型
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // 展示组合标志的用法
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // 保存工作簿
                workbook.Save("ContentMarkTypeDemo.xlsx");
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

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


