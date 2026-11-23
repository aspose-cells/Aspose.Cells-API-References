---
title: "DataModelRelationshipCollection.Item"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataModelRelationshipCollection 属性。获取关系"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

获取关系。

```csharp
public DataModelRelationship this[int index] { get; }
```

| 参数 | 描述 |
| --- | --- |
| 索引 | 索引。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // 创建一个新工作簿（空数据模型）
            Workbook workbook = new Workbook();

            try
            {
                // 从工作簿获取 DataModelRelationshipCollection（如果没有数据模型可能为 null）
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;

                if (relationships == null)
                {
                    Console.WriteLine("The workbook does not contain a data model.");
                }
                else if (relationships.Count == 0)
                {
                    Console.WriteLine("The data model exists but contains no relationships.");
                }
                else
                {
                    // 使用 Item（索引器）属性读取第一个关系
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // 保存工作簿（可选，仅用于演示代码端到端运行）
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


