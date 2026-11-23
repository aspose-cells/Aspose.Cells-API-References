---
title: "CustomProperty.BinaryValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CustomProperty 属性。获取和设置自定义属性的二进制值"
type: docs
url: /zh/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

获取和设置自定义属性的二进制值。

```csharp
public byte[] BinaryValue { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加具有示例值的自定义属性
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // 检索自定义属性
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // 显示自定义属性的 Name 和 Value
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // 注意：CustomProperty 的反射不包括 BinaryValue 属性。
                // 可用的基于字符串的值通过 'Value' 属性访问。

                // 保存工作簿（可选）
                workbook.Save("BinaryValueDemo.xlsx");
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


