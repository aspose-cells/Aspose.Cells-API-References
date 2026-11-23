---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。用于渲染 Emf 元文件的设置"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

用于渲染 Emf 元文件的设置。

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### 备注

标识为 “EMF+ Dual” 的 EMF 元文件可以同时包含 EMF+ 记录和 EMF 记录。可以使用任意类型的记录来渲染图像、仅使用 EMF+ 记录，或仅使用 EMF 记录。当设置 EmfPlusPrefer 时，渲染页面时将解析 EMF+ 记录；否则仅解析 EMF 记录。默认值为 EmfOnly。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // 创建用于 EMF 演示的图像
            worksheet.Pictures.Add(10, 10, "example.png");

            // 使用 PdfSaveOptions 配置带有 EMF 设置的保存选项
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // 使用 EMF 设置保存工作簿
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### 另请参见

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


