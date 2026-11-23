---
title: "CustomProperty.StringValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CustomProperty 属性。返回或设置自定义属性的值"
type: docs
url: /zh/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

返回或设置自定义属性的值。

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### 备注

注意：此成员现已过时。请改用 CustomProperty.Value 属性。此属性将在自 2010 年 6 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 添加具有字符串值的自定义属性
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // 检索自定义属性
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // 显示 StringValue 属性（读取操作）
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // 为 StringValue 属性设置新值
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // 保存工作簿
                workbook.Save("StringValueDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


