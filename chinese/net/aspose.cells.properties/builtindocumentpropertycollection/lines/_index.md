---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "BuiltInDocumentPropertyCollection 属性。表示文档中行数的估计值"
type: docs
url: /zh/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

表示文档中行数的估计值。

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### 备注

当您修改文档时，Aspose.Cells 不会更新此属性。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问内置文档属性
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // 显示当前 Lines 值（文档中行数的估计）
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // 为 Lines 属性设置新值
            properties.Lines = 150;
            
            // 添加一些内容以演示该属性的用途
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // 保存工作簿
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // 注意：Lines 属性是估计值，且不会随实际内容自动更新
            // 它主要用于文档元数据目的
        }
    }
}
```

### 另请参见

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


