---
title: Cells.InsertRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Inserts a new row into the worksheet
type: docs
url: /net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Inserts a new row into the worksheet.

```csharp
public void InsertRow(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |

### Examples

```csharp
// Called: cells.InsertRow(7);
public void Cells_Method_InsertRow()
{
    caseName = "testInsertValiadtion_004";
    Workbook workbook = new Workbook(Constants.sourcePath + "insertDelete\\testValiadtion.xls");
    Worksheet sheet = workbook.Worksheets[0];
    Cells cells = sheet.Cells;
    cells.InsertRow(7);

    checkInsertValiadtion_003(workbook);
    workbook.Save(Constants.destPath + "testInsertValiadtion.xls");
    workbook = new Workbook(Constants.destPath + "testInsertValiadtion.xls");
    checkInsertValiadtion_003(workbook);
    workbook.Save(Constants.destPath + "testInsertValiadtion.xlsx");
    workbook = new Workbook(Constants.destPath + "testInsertValiadtion.xlsx");
    checkInsertValiadtion_003(workbook);
    workbook.Save(Constants.destPath + "testInsertValiadtion.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testInsertValiadtion.xml");
    checkInsertValiadtion_003(workbook);
    workbook.Save(Constants.destPath + "testInsertValiadtion.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


