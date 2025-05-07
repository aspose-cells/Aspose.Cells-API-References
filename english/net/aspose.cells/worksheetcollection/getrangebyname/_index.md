---
title: WorksheetCollection.GetRangeByName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets Range object by predefined name
type: docs
url: /net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Gets Range object by pre-defined name.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range. |

### Return Value

Range object.

Returns null if the named range does not exist.

### Examples

```csharp
// Called: Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("DUP_Project");
[Test]
        public void Method_String_()
        {
            string filePath = Constants.sourcePath + "CellsNet31068.xlsx";

            WorkbookDesigner designer = new WorkbookDesigner();
            Workbook workbook = new Workbook(filePath);
            designer.Workbook = workbook;

            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("DUP_Project");
            Worksheet worksheet = range.Worksheet;

            Cells cells = range.Worksheet.Cells;

            cells.DeleteRange(range.FirstRow, range.FirstColumn, range.FirstRow + range.RowCount - 1, range.FirstColumn + range.ColumnCount - 1, ShiftType.Left);


            workbook.Save(Constants.destPath + "CellsNet31068.xlsx"); 

        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Gets [`Range`](../../range/) by pre-defined name or table's name

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range or table's name. |
| currentSheetIndex | Int32 | The sheet index. -1 represents global . |
| includeTable | Boolean | Indicates whether checking all tables. |

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


