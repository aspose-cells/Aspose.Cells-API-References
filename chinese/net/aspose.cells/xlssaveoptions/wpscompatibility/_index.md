---
title: "XlsSaveOptions.WpsCompatibility"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XlsSaveOptions 属性。指示是否使 xls 更兼容 WPS"
type: docs
url: /zh/net/aspose.cells/xlssaveoptions/wpscompatibility/
---
## XlsSaveOptions.WpsCompatibility property

指示是否使 xls 更兼容 WPS。

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### 备注

注意：此成员已过时。请改用 WorkbookSetting.WpsCompatibility 属性。此方法将在自 2025 年 12 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // 创建示例工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // 设置具有 WPS 兼容性的保存选项
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.WpsCompatibility = true;
            
            // 保存工作簿
            workbook.Save("output_with_wps_compatibility.xls", saveOptions);
            
            Console.WriteLine("File saved with WPS compatibility enabled.");
        }
    }
}
```

### 另请参见

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


