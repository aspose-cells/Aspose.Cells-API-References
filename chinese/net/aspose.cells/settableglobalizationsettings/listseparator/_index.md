---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 属性。获取函数等的列表参数分隔符"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

获取列表、函数参数等的分隔符。

```csharp
public override char ListSeparator { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建 SettableGlobalizationSettings 的实例
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // 显示当前的 ListSeparator 值（大多数区域的默认是逗号）
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // 设置新的 ListSeparator 值（例如，分号）
            settings.SetListSeparator(';');
            
            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;
            
            // 演示 ListSeparator 在公式解析中的效果
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // 创建使用列表分隔符的公式
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // 公式在解析时将使用自定义的列表分隔符
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // 保存工作簿
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


