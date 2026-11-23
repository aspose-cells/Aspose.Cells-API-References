---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取 Hours 的本地文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

获取 "Hours" 的本地文本。

```csharp
public virtual string GetTextOfHours()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfHoursDemo
    {
        public static void Run()
        {
            // 创建 PivotGlobalizationSettings 的实例
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // 演示 GetTextOfHours 方法
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // 相关时间方法的额外演示
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


