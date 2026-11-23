---
title: "DataModel.Relationships"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataModel 属性。获取数据模型中表的所有关系"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

获取数据模型中表的所有关系。

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelPropertyRelationshipsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            try
            {
                // 从工作簿访问 DataModel
                DataModel dataModel = workbook.DataModel;

                // 显示 Relationships 属性的当前值（只读）
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // 遍历关系（如果存在）
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // 保存工作簿
                workbook.Save("RelationshipsDemo.xlsx");
                Console.WriteLine("Relationships demonstration completed successfully.");
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

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


