---
title: "WebWorksheets.ImportDataView"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebWorksheets 方法。 从 DataView 导入。 自动使用 DataViews 表名创建工作表。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webworksheets/importdataview/
---
## ImportDataView(DataView, TableItemStyle, TableItemStyle) {#importdataview}

从 DataView 导入。自动使用 DataView 的表名创建工作表。

```csharp
public void ImportDataView(DataView dataView, TableItemStyle colHeaderStyle, 
    TableItemStyle dataStyle)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataView | DataView | DataView 对象。 |
| colHeaderStyle | TableItemStyle | 指定 dataview 标题栏的样式。 |
| dataStyle | TableItemStyle | 指定数据区域的样式。 |

### 另请参见

* class [TableItemStyle](../../../aspose.cells.gridweb/tableitemstyle/)
* class [WebWorksheets](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## ImportDataView(DataView, TableItemStyle, TableItemStyle, string, int, int) {#importdataview_1}

从 DataView 导入到指定的工作表和位置。

```csharp
public void ImportDataView(DataView dataView, TableItemStyle colHeaderStyle, 
    TableItemStyle dataStyle, string sheetName, int row, int column)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataView | DataView | DataView 对象。 |
| colHeaderStyle | TableItemStyle | 指定 dataview 标题栏的样式。 |
| dataStyle | TableItemStyle | 指定数据区域的样式。 |
| sheetName | String | 指定工作表名称。如果工作表不存在，将为您创建。 |
| 行 | Int32 | 指定导入位置。 |
| 列 | Int32 | 指定导入位置。 |

### 另请参见

* class [TableItemStyle](../../../aspose.cells.gridweb/tableitemstyle/)
* class [WebWorksheets](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


