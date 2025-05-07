---
title: ListObject.Resize
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Resize the range of the list object
type: docs
url: /net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Resize the range of the list object.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row index of the new range. |
| startColumn | Int32 | The start column index of the new range. |
| endRow | Int32 | The end row index of the new range. |
| endColumn | Int32 | The end column index of the new range. |
| hasHeaders | Boolean | Whether this table has headers. |

### Examples

```csharp
// Called: table.Resize(table.StartRow, table.StartColumn, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wbSource = new Workbook(Constants.sourcePath + "CellsNet45529.xlsx");
            Worksheet sheet = wbSource.Worksheets["Test"];

            ListObject table = sheet.ListObjects[0];

            table.Resize(table.StartRow, table.StartColumn, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true);

            //   wbSource.Save(tgtFilePath); 
           AssertHelper.AreEqual(Color.FromArgb(88, 88, 90), sheet.Cells["B19"].GetStyle().ForegroundColor);
            Util.SaveManCheck(wbSource, "Shape", "CellsNet45529.xlsx");
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


