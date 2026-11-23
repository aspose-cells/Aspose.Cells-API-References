---
title: "类 PivotAreaCollection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotAreaCollection 类。表示数据透视区域的列表"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareacollection/
---
## PivotAreaCollection class

表示数据透视区域的列表。

```csharp
public class PivotAreaCollection : CollectionBase<PivotArea>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotareacollection/item/) { get; } | 获取一个[`PivotArea`](../pivotarea/)对象; |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add_1)(CellArea) | 基于透视表视图添加区域。 |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add)(PivotArea) | (**已弃用。**) 添加数据透视区域。 |
| [AddPivotArea](../../aspose.cells.pivot/pivotareacollection/addpivotarea/)(PivotArea) | 将数据透视区域添加到此集合中。 |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotArea) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotArea, IComparer&lt;PivotArea&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotArea, IComparer&lt;PivotArea&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotArea) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotArea[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotArea[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotArea[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotArea&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotArea&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotArea&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotArea&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea, int, int) |  |
| [RemoveAt](../../aspose.cells.pivot/pivotareacollection/removeat/#removeat)(int) | 删除一个数据透视条件格式化区域设置。（2 种方法） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaCollectionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表创建示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue(1200);

            // 添加数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 为数据透视区域创建单元格区域
            CellArea dataArea = new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 1 };
            CellArea headerArea = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 1 };

            // 获取数据透视区域集合
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(dataArea);

            // 添加数据透视区域
            pivotAreas.Add(dataArea);
            pivotAreas.Add(headerArea);

            // 显示所有数据透视区域
            Console.WriteLine("Pivot Areas Count: " + pivotAreas.Count);
            for (int i = 0; i < pivotAreas.Count; i++)
            {
                CellArea[] areas = pivotAreas[i].GetCellAreas();
                foreach (CellArea area in areas)
                {
                    Console.WriteLine($"Area {i}: ({area.StartRow},{area.StartColumn}) to ({area.EndRow},{area.EndColumn})");
                }
            }

            // 删除一个区域
            pivotAreas.RemoveAt(0);
            Console.WriteLine("\nAfter removal - Pivot Areas Count: " + pivotAreas.Count);

            // 保存工作簿
            workbook.Save("PivotAreaCollectionDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotArea](../pivotarea/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


