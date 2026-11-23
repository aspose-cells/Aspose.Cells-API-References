---
title: "BuiltInDocumentPropertyCollection.Paragraphs"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "BuiltInDocumentPropertyCollection 属性。表示文档中段落数量的估计值"
type: docs
url: /zh/net/aspose.cells.properties/builtindocumentpropertycollection/paragraphs/
---
## BuiltInDocumentPropertyCollection.Paragraphs property

表示文档中段落数量的估计值。

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Paragraphs { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyParagraphsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问内置文档属性
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // 显示当前 Paragraphs 值（已弃用属性）
            Console.WriteLine("Current Paragraphs value: " + properties.Paragraphs);

            // 为 Paragraphs 设置新值（已弃用属性）
            properties.Paragraphs = 15;
            Console.WriteLine("Updated Paragraphs value: " + properties.Paragraphs);

            // 添加一些内容以演示属性效果
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is paragraph 1");
            worksheet.Cells["A2"].PutValue("This is paragraph 2");
            worksheet.Cells["A3"].PutValue("This is paragraph 3");

            // 保存工作簿
            workbook.Save("PropertyParagraphsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


