---
title: "LoadOptions.StandardFont"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LoadOptions 属性。设置默认的标准字体名称"
type: docs
url: /zh/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

设置默认的标准字体名称

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### 备注

注意：此成员现已过时。请改用 DefaultStyleSettings。此属性将在自 2022 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // 在内存中创建示例 Excel 文件
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // 使用 StandardFont 设置加载选项
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // 使用指定的字体加载工作簿
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // 通过检查默认样式演示已设置字体
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### 另请参见

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


