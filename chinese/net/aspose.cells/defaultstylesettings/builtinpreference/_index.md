---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DefaultStyleSettings 属性。指示当样式同时定义内置数字和自定义模式时，数字格式属性是否更可取。默认值为 false，这意味着默认情况下只要该样式的自定义模式非空，就会使用自定义模式来格式化值。"
type: docs
url: /zh/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

指示当样式同时定义内置数字和自定义模式时，数字格式属性是否更可取。默认值为 false，这意味着默认情况下只要该样式的自定义模式非空，就会使用自定义模式来格式化值。

```csharp
public bool BuiltInPreference { get; set; }
```

### 备注

从现有模板文件加载工作簿时，可能会为同一样式同时定义内置数字和自定义模式。此属性决定在使用该样式格式化值时应使用内置数字还是自定义模式。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问默认样式设置
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // 演示 BuiltInPreference 属性
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // 应用于工作表
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // 保存工作簿
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


