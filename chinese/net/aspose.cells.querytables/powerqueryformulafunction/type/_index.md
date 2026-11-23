---
title: "PowerQueryFormulaFunction.Type"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PowerQueryFormulaFunction 属性。获取 Power Query 公式的类型"
type: docs
url: /zh/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

获取 Power Query 公式的类型。

```csharp
public override PowerQueryFormulaType Type { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 Power Query 公式函数
            // 由于无法直接创建，我们需要从某处获取它
            // 演示时，我们仅展示如何访问 Type 属性
            // （在实际使用中，您会从现有集合中获取此项）
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // 由于也无法直接创建 QueryTable，我们将跳过该部分
            QueryTable queryTable = null; // Can't instantiate directly
            
            // 无法以这种方式向查询表集合添加 - 它是只读的
            // worksheet.QueryTables[0] = queryTable; // 删除此行
            
            // 演示时，我们仅展示如果有函数时将使用的输出格式
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // 保存结果
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


