---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取月份的本地文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

获取 "Months" 的本地文本。

```csharp
public virtual string GetTextOfMonths()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMonthsDemo
    {
        public static void Run()
        {
            // 创建自定义全局化设置
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // 演示 GetTextOfMonths
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // 返回 "Months" 的自定义本地化文本
            return "Custom Months Label";
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


