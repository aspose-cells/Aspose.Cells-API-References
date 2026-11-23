---
title: "BuiltInDocumentPropertyCollection.Bytes"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "BuiltInDocumentPropertyCollection 属性。表示文档中字节数的估计值"
type: docs
url: /zh/net/aspose.cells.properties/builtindocumentpropertycollection/bytes/
---
## BuiltInDocumentPropertyCollection.Bytes property

表示文档中字节数的估计值。

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问内置文档属性
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // 显示当前 Bytes 值（文档大小的估计）
            Console.WriteLine("Current Bytes value: " + properties.Bytes);

            // 添加一些内容以影响大小
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data to increase document size");
            for (int i = 2; i <= 100; i++)
            {
                worksheet.Cells["A" + i].PutValue("Line " + i);
            }

            // 手动更新 Bytes 属性（尽管通常会自动计算）
            properties.Bytes = 5000;
            Console.WriteLine("Updated Bytes value: " + properties.Bytes);

            // 保存工作簿以在保存的文件中查看该属性
            workbook.Save("PropertyBytesDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


