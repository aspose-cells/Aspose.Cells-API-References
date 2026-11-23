---
title: "PowerQueryFormula.Type"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PowerQueryFormula 属性。获取此 Power Query 公式的类型"
type: docs
url: /zh/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

获取此 Power Query 公式的类型。

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 获取现有公式（新工作簿中无公式）以演示 Type 属性
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // 在实际场景中，若存在公式，我们会检查它们的类型
            Console.WriteLine("Power Query Formula Types:");
            
            // 这演示了检查 Type 属性
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // 为演示目的，在不存在公式时添加输出
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // 保存工作簿
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### 另请参见

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


