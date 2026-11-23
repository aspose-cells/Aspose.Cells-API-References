---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的标准文本获取内置 Name 的区域相关文本"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

根据给定的标准文本获取内置名称的区域设置相关文本。

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| standardName | String | 标准（en-US 区域）内置 Name 的文本。 |

### 返回值

区域相关文本。区域由使用此设置的工作簿指定。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 SettableGlobalizationSettings 的实例
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // 使用标准内置名称调用 GetLocalBuiltInName 方法
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // 显示结果
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // 为标准内置名称设置自定义本地名称
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // 设置后再次获取本地名称
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


