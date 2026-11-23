---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取指定受保护名称的文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

获取指定受保护名称的文本。

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| protectedName | String | PivotTable 中的受保护名称。 |

### 返回值

PivotTable 的本地受保护名称。

### 备注

在 Microsoft Excel 中，某些名称不能用作数据透视表中 PivotFields 的名称。这些名称因地区而异，用户可以根据所使用的地区显式指定它们。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectedNameWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // 创建 PivotGlobalizationSettings 的实例
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // 定义受保护名称以检索其文本
                string protectedName = "SensitiveData";

                // 调用 GetTextOfProtectedName 方法
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // 输出结果
                Console.WriteLine($"Text for protected name \"{protectedName}\": {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


