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
// Called: cells.InsertRow(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "insertDelete\\insertRow\\insertRow_ConditionalFormatting_001.xls");
            Cells cells = workbook.Worksheets["AsposeResult"].Cells;
            cells.InsertRow(0);

            CheckInsertRow_ConditionalFormatting_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRow.xls");
            workbook = new Workbook(Constants.destPath + " testInsertRow.xls");
            CheckInsertRow_ConditionalFormatting_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRow.xlsx");
            workbook = new Workbook(Constants.destPath + " testInsertRow.xlsx");
            CheckInsertRow_ConditionalFormatting_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRow.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + " testInsertRow.xml");
            CheckInsertRow_ConditionalFormatting_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRow.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


