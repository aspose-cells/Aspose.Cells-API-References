---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PowerQueryFormulaCollection 方法。按名称删除 Power Query 公式"
type: docs
url: /zh/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

按名称删除 Power Query 公式。

```csharp
public void RemoveBy(string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | String | Power Query 公式的名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 访问 PowerQueryFormulaCollection（假设它存在于工作簿中）
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // 添加一个待删除的示例公式（这通常来自现有数据）
                string formulaName = "SampleFormula";
                
                // 使用公式名称调用 RemoveBy
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // 保存工作簿
                workbook.Save("RemoveByWithStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


