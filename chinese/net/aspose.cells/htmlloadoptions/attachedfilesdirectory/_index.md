---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlLoadOptions 属性。附加文件将保存到的目录"
type: docs
url: /zh/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

附加文件将保存到的目录。

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### 备注

注意：此成员已过时。请改用 HtmlLoadOptions.StreamProvider 属性。此属性将在自 2014 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // 创建 HtmlLoadOptions 的实例
            HtmlLoadOptions options = new HtmlLoadOptions();

            // 设置附加文件的目录
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // 使用指定的选项将 HTML 文件加载到工作簿中
            Workbook workbook = new Workbook("input.html", options);

            // 将工作簿保存为 Excel 文件
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


