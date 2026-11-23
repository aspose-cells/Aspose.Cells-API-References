---
title: "CalculationOptions.LinkedDataSources"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CalculationOptions 属性。指定公式中使用的外部链接的数据源"
type: docs
url: /zh/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

指定公式中使用的外部链接的数据源。

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### 备注

类似于 [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/)，在此您可以指定用于计算的公式中使用的外部链接的数据源，特别是那些在 INDIRECT 函数中使用的链接。对于在 INDIRECT 函数中使用的外部链接，它们不被视为工作簿的外部链接的一部分，且无法通过 [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/) 进行更新。这些工作簿与外部链接的匹配由 [`FileName`](../../workbook/filename/) 和 [`DataSource`](../../externallink/datasource/) 决定。因此，请确保每个工作簿的 [`FileName`](../../workbook/filename/) 已使用适当的值进行指定（通常应与相应的 [`DataSource`](../../externallink/datasource/) 相同），以便它们能够按预期链接。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // 创建包含数据的外部工作簿
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // 在外部工作簿中添加命名范围
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // 创建主工作簿
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // 设置引用外部工作簿的公式
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // 使用 LinkedDataSources 计算公式
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### 另请参见

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


