---
title: "ReferredArea.SheetNames"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ReferredArea 属性。此实例引用的所有工作表名称"
type: docs
url: /zh/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

此实例引用的所有工作表名称。

```csharp
public string[] SheetNames { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些数据以创建公式引用
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // 计算公式以获取引用
            workbook.CalculateFormula();

            // 从 A3 单元格的公式获取引用区域
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // 显示 SheetNames 属性
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // 添加另一个工作表并创建跨工作表引用
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // 再次计算公式
            workbook.CalculateFormula();

            // 从跨工作表公式获取引用区域
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // 显示跨工作表引用的 SheetNames
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // 保存工作簿
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


