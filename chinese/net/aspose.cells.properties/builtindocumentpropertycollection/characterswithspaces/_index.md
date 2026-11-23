---
title: "BuiltInDocumentPropertyCollection.CharactersWithSpaces"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "BuiltInDocumentPropertyCollection 属性。表示文档中包括空格的字符数量的估计值"
type: docs
url: /zh/net/aspose.cells.properties/builtindocumentpropertycollection/characterswithspaces/
---
## BuiltInDocumentPropertyCollection.CharactersWithSpaces property

表示文档中字符数量（包括空格）的估计值。

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CharactersWithSpaces { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersWithSpacesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问内置文档属性
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // 显示当前 CharactersWithSpaces 值
            Console.WriteLine("Current CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // 为 CharactersWithSpaces 设置新值
            properties.CharactersWithSpaces = 1500;
            Console.WriteLine("Updated CharactersWithSpaces value: " + properties.CharactersWithSpaces);
            
            // 添加一些内容以演示属性效果
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            worksheet.Cells["A2"].PutValue("The CharactersWithSpaces property represents estimated character count including spaces.");
            
            // 保存工作簿
            workbook.Save("PropertyCharactersWithSpacesDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


