---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookSettings 属性。获取和设置图像的默认分辨率"
type: docs
url: /zh/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

获取和设置图像的默认分辨率。

```csharp
public int DefaultImageResolution { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 设置默认图像分辨率
            workbook.Settings.DefaultImageResolution = 300;
            
            // 添加工作表并插入图像
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // 保存工作簿
            workbook.Save("output.xlsx");
            
            // 验证默认图像分辨率
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### 另请参见

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


