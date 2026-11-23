---
title: "WebWorksheet.CreateSubtotal"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebWorksheet 方法。在工作表中创建小计。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webworksheet/createsubtotal/
---
## WebWorksheet.CreateSubtotal method

在工作表中创建小计。

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnNameRowIndex | Int32 | 列名行的行索引。 |
| dataRows | Int32 | 数据行的数量。 |
| groupByColumnIndex | Int32 | 要分组的列的列索引。 |
| subtotalFunction | SubtotalFunction | 小计函数类型。 |
| subtotalColumnIndexList | Int32[] | 要进行小计的列索引。 |
| functionLabel | String | 小计函数的标签。 |
| grandCellStyle | GridTableItemStyle | 总计行的样式。 |
| subtotalCellStyle | GridTableItemStyle | 小计行的样式。 |
| numberType | NumberType | 小计结果单元格的数字类型。 |
| customString | String | 小计结果单元格的自定义格式字符串。可以为 null。 |

### 另请参见

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


