---
title: "DataModel.Tables"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataModel 属性。获取数据模型中的所有表"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

获取数据模型中的所有表。

```csharp
public DataModelTableCollection Tables { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class DataModelPropertyTablesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook wb = new Workbook();
            
            // 访问数据模型
            DataModel dataModel = wb.DataModel;
            
            // 获取表集合并显示计数
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // 加载带有数据模型的示例工作簿
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // 访问表集合
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // 遍历表
                foreach (DataModelTable table in tables)
                {
                    Console.WriteLine($"Table name: {table.Name}");
                }
            }
            else
            {
                Console.WriteLine($"Sample file '{sourceFile}' not found. Create an Excel file with data model to see tables information.");
            }
        }
    }
}
```

### 另请参见

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


