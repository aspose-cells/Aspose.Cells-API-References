---
title: "枚举 PowerQueryFormulaType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaType 枚举。表示 Power Query 公式的类型"
type: docs
url: /zh/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

表示 Power Query 公式的类型。

```csharp
public enum PowerQueryFormulaType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Formula | `0` | 公式 Power Query 公式。 |
| Function | `1` | 函数 Power Query 公式。 |
| Parameter | `2` | 参数 Power Query 公式。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaTypeDemo
    {
        public static void Run()
        {
            try
            {
                // 演示 PowerQueryFormulaType 枚举的所有值
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // 显示枚举值及其数值表示
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // 演示枚举比较
                if (formulaType == PowerQueryFormulaType.Formula)
                {
                    Console.WriteLine("Successfully identified Formula type");
                }

                if (functionType == PowerQueryFormulaType.Function)
                {
                    Console.WriteLine("Successfully identified Function type");
                }

                if (parameterType == PowerQueryFormulaType.Parameter)
                {
                    Console.WriteLine("Successfully identified Parameter type");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


