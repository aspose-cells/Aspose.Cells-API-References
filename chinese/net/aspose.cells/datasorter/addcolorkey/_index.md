---
title: "DataSorter.AddColorKey"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataSorter 方法。添加颜色排序键"
type: docs
url: /zh/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

添加颜色排序键。

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 键 | Int32 | 已排序列的索引（绝对位置，列 A 为 0，B 为 1，...） |
| 类型 | SortOnType | 已排序颜色值的类型。 |
| 顺序 | SortOrder | 排序顺序。 |
| 颜色 | Color | 自定义排序颜色。 |

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加带颜色单元格的示例数据
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // 将颜色应用于单元格
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // 创建数据排序器并添加颜色键
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // 对数据进行排序
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // 输出已排序的值（用于演示）
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### 另请参见

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


