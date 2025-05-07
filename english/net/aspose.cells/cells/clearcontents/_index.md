---
title: Cells.ClearContents
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears contents of a range
type: docs
url: /net/aspose.cells/cells/clearcontents/
---
## ClearContents(CellArea) {#clearcontents}

Clears contents of a range.

```csharp
public void ClearContents(CellArea range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

### Examples

```csharp
// Called: cells.ClearContents(ca);
private void Method_CellArea_(Worksheet sheet, string fml, CellArea expected, string[] res)
        {
            Cells cells = sheet.Cells;
            Cell cell = cells[expected.StartRow, expected.StartColumn];
            CellArea ca = cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            AssertHelper.checkCellArea(expected, ca, fml);
            CheckArrayFormula(fml, cells, ca, "");
            CheckResult(res, cells, ca, fml);
            cells.ClearContents(ca);
            ca = cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), false);
            AssertHelper.checkCellArea(expected, ca, fml);
            CheckArrayFormula(fml, cells, ca, "");
            sheet.Workbook.CalculateFormula();
            CheckResult(res, cells, ca, fml);
            cells.ClearContents(ca);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearContents(int, int, int, int) {#clearcontents_1}

Clears contents of a range.

```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |

### Examples

```csharp
// Called: cells.ClearContents(0, 0, 2, 2);
[Test]
        public void Method_Int32_()
        {
            caseName = "testClearContents_002";
            Workbook workbook = new Workbook(Constants.sourcePath + "Cells\\cellsClearContents_001.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.ClearContents(0, 0, 2, 2);

            checkClearContents_001(workbook);
            workbook.Save(Constants.destPath + "testClearContents.xls");
            workbook = new Workbook(Constants.destPath + "testClearContents.xls");
            checkClearContents_001(workbook);
            workbook.Save(Constants.destPath + "testClearContents.xlsx");
            workbook = new Workbook(Constants.destPath + "testClearContents.xlsx");
            checkClearContents_001(workbook);
            workbook.Save(Constants.destPath + "testClearContents.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testClearContents.xml");
            checkClearContents_001(workbook);
            workbook.Save(Constants.destPath + "testClearContents.xls");        
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


