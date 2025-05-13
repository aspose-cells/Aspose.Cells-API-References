---
title: Cells.GroupColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Groups columns
type: docs
url: /net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Groups columns.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be grouped. |
| lastIndex | Int32 | The last column index to be grouped. |

### Examples

```csharp
// Called: cells.GroupColumns(0, 255);
public void Cells_Method_GroupColumns()
{
    caseName = "testGroupColumns_003";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells.GroupColumns(0, 255);

    workbook.Save(Constants.destPath + "testGroupColumns.xls");
    workbook = new Workbook(Constants.destPath + "testGroupColumns.xls");
    workbook.Save(Constants.destPath + "testGroupColumns.xlsx");
    workbook = new Workbook(Constants.destPath + "testGroupColumns.xlsx");
    workbook.Save(Constants.destPath + "testGroupColumns.xls"); 
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Groups columns.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be grouped. |
| lastIndex | Int32 | The last column index to be grouped. |
| isHidden | Boolean | Specifies if the grouped columns are hidden. |

### Examples

```csharp
// Called: cells.GroupColumns(5, 3, true);
public void Cells_Method_GroupColumns()
{
    caseName = "testGroupColumns_002";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells.GroupColumns(5, 3, true);
    workbook.Save(Constants.destPath + "testGroupColumns.xls");
    workbook = new Workbook(Constants.destPath + "testGroupColumns.xls");
    workbook.Save(Constants.destPath + "testGroupColumns.xlsx");
    workbook = new Workbook(Constants.destPath + "testGroupColumns.xlsx");
    workbook.Save(Constants.destPath + "testGroupColumns.xls"); 
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


