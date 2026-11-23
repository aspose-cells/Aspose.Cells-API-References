---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookSettings 属性。指示是否丢弃编辑的图像数据"
type: docs
url: /zh/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

指示是否丢弃编辑的图像数据。

```csharp
public bool DiscardImageEditData { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加图像
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // 将 DiscardImageEditData 设置为 true（默认是 false）
            workbook.Settings.DiscardImageEditData = true;
            
            // 保存工作簿
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // 验证设置已应用
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### 另请参见

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


