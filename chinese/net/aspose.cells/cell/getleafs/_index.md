---
title: "Cell.GetLeafs"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 方法。获取所有直接引用此单元格并在此单元格被修改时需要更新的单元格"
type: docs
url: /zh/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

获取所有直接引用此单元格并在此单元格被修改时需要更新的单元格。

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### 返回值

枚举器，用于枚举所有依赖项（Cell）

### 备注

注意：此类现已过时。请改用 Cell.GetDependentsInCalculation(bool) 来获取计算链中的所有依赖项。此属性将在自 2022 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些数据和公式以创建依赖关系
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // 获取具有依赖项的单元格
                Cell cell = worksheet.Cells["B1"];

                // 调用 GetLeafs 获取所有直接引用此单元格的单元格
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // 保存工作簿
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

获取此单元格被修改时将被更新的所有单元格。

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 递归 | 布尔 | 是否返回那些不直接引用此单元格而是引用此单元格的其他叶子单元格的叶子 |

### 返回值

枚举器，用于枚举所有依赖项（Cell）

### 备注

注意：此类现已过时。请改用 Cell.GetDependentsInCalculation(bool) 来获取计算链中的所有依赖项。此属性将在自 2022 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些带公式的数据以创建依赖关系
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // 获取具有依赖项的单元格
                Cell cell = worksheet.Cells["A1"];

                // 调用 GetLeafs 并将 recursive 参数设置为 true
                IEnumerator leafs = cell.GetLeafs(true);

                // 显示结果
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // 保存工作簿
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


