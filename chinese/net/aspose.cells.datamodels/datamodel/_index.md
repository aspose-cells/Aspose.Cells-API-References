---
title: "类 DataModel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.DataModels.DataModel 类。表示数据模型"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

表示数据模型。

```csharp
public class DataModel
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | 获取数据模型中表的所有关系。 |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | 获取数据模型中的所有表。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 从工作簿获取 DataModel，而不是创建新实例
            DataModel dataModel = workbook.DataModel;

            // 演示访问表和关系（只读属性）
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // 注意：由于表和关系是只读集合，
            // 我们只能访问现有项，但不能直接修改它们

            // 保存工作簿（DataModel 通常在 Aspose.Cells 内部使用）
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


