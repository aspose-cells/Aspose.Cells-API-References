---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取数据透视字段的显示名称。默认格式为 Sum Of Field"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

获取数据透视字段的显示名称。默认格式为 "Sum Of Field"。

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 函数 | ConsolidationFunction | 该函数用于汇总透视字段的值。 |
| 名称 | String | 透视字段的原始名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // 创建 PivotGlobalizationSettings 的实例
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // 为 GetNameOfDataField 方法定义参数
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // 调用 GetNameOfDataField 方法
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // 输出结果
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


