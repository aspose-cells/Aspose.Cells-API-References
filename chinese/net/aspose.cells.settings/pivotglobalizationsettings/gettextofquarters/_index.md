---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取 Quarters 的本地文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

获取 "Quarters" 的本地文本。

```csharp
public virtual string GetTextOfQuarters()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfQuartersDemo
    {
        public static void Run()
        {
            // 创建全局化设置实例
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // 演示 GetTextOfQuarters 方法
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // 显示上下文的其他相关时间段标签
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


