---
title: "WorksheetCollection.SensitivityLabels"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorksheetCollection 属性。表示所有敏感度标签"
type: docs
url: /zh/net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

表示所有敏感度标签。

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metas;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertySensitivityLabelsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问工作表集合
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // 添加敏感度标签
            int index = worksheets.SensitivityLabels.Add(
                "{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
                true,                                       // IsEnabled
                SensitivityLabelAssignmentType.Standard,     // AssignmentType
                "contoso-site",                             // SiteId
                SensitivityLabelMarkType.Header              // MarkType
            );
            
            // 验证已添加的标签
            SensitivityLabel label = worksheets.SensitivityLabels[index];
            Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
            
            // 保存工作簿
            workbook.Save("SensitivityLabelsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


