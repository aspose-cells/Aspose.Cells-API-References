---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指示输出的 HTML 是否兼容移动设备。默认值为 false"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

指示输出的 HTML 是否兼容移动设备。默认值为 false。

```csharp
public bool IsMobileCompatible { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // 创建 HTML 保存选项
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // 设置移动兼容性
            saveOptions.IsMobileCompatible = true;

            // 在启用移动兼容性的情况下保存
            workbook.Save("MobileCompatible.html", saveOptions);

            // 更改为不兼容移动设备
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


