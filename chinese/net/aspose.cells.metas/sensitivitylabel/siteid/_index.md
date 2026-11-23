---
title: "SensitivityLabel.SiteId"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SensitivityLabel 属性。表示对应于描述敏感度标签的敏感度标签策略的 Azure Active Directory（Azure AD）站点标识符"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

表示对应于描述敏感度标签的敏感度标签策略的 Azure Active Directory（Azure AD）站点标识符。

```csharp
public string SiteId { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertySiteIdDemo
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

                // 演示获取初始 SiteId 值
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // 将 SiteId 设置为示例 Azure AD 站点标识符
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // 更改 SiteId 以演示它是可读写的
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // 显示 SiteId 与其他属性的关联方式
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // 保存工作簿
                workbook.Save("SiteIdDemo.xlsx");
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


