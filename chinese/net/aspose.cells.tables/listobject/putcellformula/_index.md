---
title: "ListObject.PutCellFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ListObject 方法。将公式写入表中的单元格"
type: docs
url: /zh/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

将公式写入表中的单元格。

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | Int32 | 表中行的偏移量。 |
| columnOffset | Int32 | 表中列的偏移量。 |
| 公式 | String | 单元格的公式。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // 添加示例数据以创建表
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // 创建列表对象（表）
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // 添加新行并设置值/公式
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // 保存工作簿
            wb.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

将公式写入表中的单元格。

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | Int32 | 表中行的偏移量。 |
| columnOffset | Int32 | 表中列的偏移量。 |
| 公式 | String | 单元格的公式。 |
| isTotalsRowFormula | 布尔 |  |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据以创建列表对象
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // 创建列表对象
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // 演示 PutCellFormula
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


