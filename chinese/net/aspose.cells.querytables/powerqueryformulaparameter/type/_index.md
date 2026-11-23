---
title: "PowerQueryFormulaParameter.Type"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PowerQueryFormulaParameter 属性。获取 Power Query 公式的类型"
type: docs
url: /zh/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

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

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 由于我们无法在不知道所需构造函数参数的情况下直接创建 PowerQueryFormulaParameter，
                // 我们将演示通过现有查询表的参数访问 Type 属性
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // 在真实场景中，您会从现有的查询表中访问此项
                // 为了演示目的，我们将展示如果有实例时如何检查类型
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // 显示 Type 属性值（只读属性）
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // 显示可能的枚举值
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // 保存工作簿
                workbook.Save("TypeDemo.xlsx");
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

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


