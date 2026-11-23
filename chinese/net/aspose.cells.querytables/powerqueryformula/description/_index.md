---
title: "PowerQueryFormula.Description"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PowerQueryFormula 属性。获取并设置 Power Query 公式的描述"
type: docs
url: /zh/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

获取并设置 Power Query 公式的描述。

```csharp
public string Description { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaPropertyDescriptionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            try
            {
                // 加载包含 Power Query 公式的现有文件
                workbook = new Workbook("example.xlsx");

                // 访问现有的 Power Query 公式
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // 显示当前 Description 值
                    Console.WriteLine("Current Description: " + formula.Description);

                    // 设置新的描述
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // 保存工作簿
                    workbook.Save("PowerQueryFormulaDescriptionDemo.xlsx");
                    Console.WriteLine("Description property demonstrated successfully.");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### 另请参见

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


