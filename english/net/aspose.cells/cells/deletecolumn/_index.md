---
title: Cells.DeleteColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes a column
type: docs
url: /net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Deletes a column.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: cells.DeleteColumn(0, true);
public void Cells_Method_DeleteColumn()
{
    caseName = "testDeleteChart_010";
    Workbook workbook = new Workbook(Constants.sourcePath + "insertDelete\\ChartsUpdateOtherRef.xls");
    Worksheet sheet = workbook.Worksheets[0];
    Chart chart = sheet.Charts[0];
    Cells cells = sheet.Cells;
    cells.DeleteRows(10, 3, true);
    cells.DeleteColumn(0, true);

    checkDeleteChart_010(workbook);
    workbook.Save(Constants.destPath + " testDeleteChart.xls");
    workbook = new Workbook(Constants.destPath + " testDeleteChart.xls");
    checkDeleteChart_010(workbook);
    workbook.Save(Constants.destPath + " testDeleteChart.xlsx");
    workbook = new Workbook(Constants.destPath + " testDeleteChart.xlsx");
    checkDeleteChart_010(workbook);
    workbook.Save(Constants.destPath + " testDeleteChart.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumn(int) {#deletecolumn}

Deletes a column.

```csharp
public void DeleteColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |

### Examples

```csharp
// Called: cells.DeleteColumn(1);
public void Cells_Method_DeleteColumn()
{
    caseName = "testDeleteValiadtion_006";
    Workbook workbook = new Workbook(Constants.sourcePath + "insertDelete\\testValiadtion.xls");
    Worksheet sheet = workbook.Worksheets[0];
    Cells cells = sheet.Cells;
    cells.DeleteColumn(1);

    checkDeleteValiadtion(workbook, 3, 1, 6, 3);
    workbook.Save(Constants.destPath + "testDeleteValiadtion.xls");
    workbook = new Workbook(Constants.destPath + "testDeleteValiadtion.xls");
    checkDeleteValiadtion(workbook, 3, 1, 6, 3);
    workbook.Save(Constants.destPath + "testDeleteValiadtion.xlsx");
    workbook = new Workbook(Constants.destPath + "testDeleteValiadtion.xlsx");
    checkDeleteValiadtion(workbook, 3, 1, 6, 3);
    workbook.Save(Constants.destPath + "testDeleteValiadtion.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testDeleteValiadtion.xml");
    checkDeleteValiadtion(workbook, 3, 1, 6, 3);
    workbook.Save(Constants.destPath + "testDeleteValiadtion.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


