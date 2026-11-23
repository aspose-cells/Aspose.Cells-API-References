---
title: "SensitivityLabelCollection.Add"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SensitivityLabelCollection 方法。添加敏感度标签"
type: docs
url: /zh/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

添加一个敏感度标签。

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| id | String | 标签的 id。 |
| isEnabled | 布尔 | 指示此敏感度标签是否已启用。 |
| methodType | SensitivityLabelAssignmentType | 分配方法类型。 |
| siteId | String | 站点的 id。 |
| markType | SensitivityLabelMarkType | 标记类型。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建一个新的 SensitivityLabelCollection
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // 使用特定参数调用 Add 方法
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // 添加一些数据以演示效果
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // 保存结果
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


