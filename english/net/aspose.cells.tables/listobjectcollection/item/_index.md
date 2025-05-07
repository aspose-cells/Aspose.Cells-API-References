---
title: ListObjectCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ListObjectCollection property. Gets the ListObject by index
type: docs
url: /net/aspose.cells.tables/listobjectcollection/item/
---
## ListObjectCollection indexer (1 of 2)

Gets the ListObject by index.

```csharp
public ListObject this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The ListObject

### Examples

```csharp
// Called: ListObject lo = workbook.Worksheets[0].ListObjects[0];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Table_001.xlsx");
            ListObject lo = workbook.Worksheets[0].ListObjects[0];
            lo.ShowHeaderRow = true;
            Assert.IsFalse(workbook.Worksheets[0].Cells["A1"].GetStyle().Font.IsBold);

            workbook.Save(Constants.destPath + "Table_001.xlsx");
        }
```

### See Also

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListObjectCollection indexer (2 of 2)

Gets the ListObject by specified name.

```csharp
public ListObject this[string tableName] { get; }
```

| Parameter | Description |
| --- | --- |
| tableName | ListObject name. |

### Return Value

The ListObject

### Examples

```csharp
// Called: ListObject table = objects["rptEquipPivot"];
[Test]
        public void Property_String_()
        {
            Workbook wbTemplate = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet57354_EquipPivot.xlsx");
            Workbook wbData = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet57354_Data.xlsx");

            Worksheet wsTemplate = wbTemplate.Worksheets[1];
            Worksheet wsData = wbData.Worksheets[0];

            DataTable dt = wsData.Cells.ExportDataTable(0, 0, wsData.Cells.LastCell.Row + 1, wsData.Cells.LastCell.Column + 1, true);

            ListObjectCollection objects = wsTemplate.ListObjects;
            ListObject table = objects["rptEquipPivot"];



            wsTemplate.Cells.DeleteRange(table.StartRow + 1, table.StartColumn, table.EndRow, table.EndColumn, ShiftType.Up);

            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = false;
            importOptions.ShiftFirstRowDown = false;
            wsTemplate.Cells.ImportData(dt, 1, 0, importOptions);
            Assert.AreEqual("=rptEquipPivot!$A$1:$CV$282", wbTemplate.Worksheets.Names["rptEquipPivot!ExternalData_1"].RefersTo);
            table.Resize(0, 0, wsTemplate.Cells.LastCell.Row, wsTemplate.Cells.LastCell.Column, true);
            Assert.AreEqual("=rptEquipPivot!$A$1:$CV$282", wbTemplate.Worksheets.Names["rptEquipPivot!ExternalData_1"].RefersTo);
            //If File.Exists(outfile) Then File.Delete(outfile)
            wbTemplate.Save(Constants.destPath + "CellsNet57354.xlsx");
        }
```

### See Also

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


