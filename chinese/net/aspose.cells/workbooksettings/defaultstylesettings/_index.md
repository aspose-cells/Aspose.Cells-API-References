---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookSettings 属性。获取此工作簿的样式相关属性的默认值设置"
type: docs
url: /zh/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

获取此工作簿的样式相关属性的默认值设置。

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### 示例

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问默认样式设置
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // 设置内置数字格式首选项
            styleSettings.BuiltInPreference = true;

            // 设置数字格式化的区域文化
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // 访问单元格并应用格式
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 设置值和样式
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // 保存工作簿
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


