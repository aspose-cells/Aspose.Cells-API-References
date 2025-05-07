---
title: Cells.ClearRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears contents and formatting of a range
type: docs
url: /net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Clears contents and formatting of a range.

```csharp
public void ClearRange(CellArea range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Clears contents and formatting of a range.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |

### Examples

```csharp
// Called: cells.ClearRange(65535, 255, 65535, 255);
[Test]
        public void Method_Int32_()
        {
            caseName = "testClearRange_005";
            Workbook workbook = new Workbook(Constants.sourcePath + "Cells\\cellsClearContents_003.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.ClearRange(65535, 255, 65535, 255);

            checkClearRange_005(workbook);
            workbook.Save(Constants.destPath + "testClearRange.xls");
            workbook = new Workbook(Constants.destPath + "testClearRange.xls");
            checkClearRange_005(workbook);
            workbook.Save(Constants.destPath + "testClearRange.xlsx");
            workbook = new Workbook(Constants.destPath + "testClearRange.xlsx");
            checkClearRange_005(workbook);
            workbook.Save(Constants.destPath + "testClearRange.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testClearRange.xml");
            checkClearRange_005(workbook);
            workbook.Save(Constants.destPath + "testClearRange.xls"); 
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


