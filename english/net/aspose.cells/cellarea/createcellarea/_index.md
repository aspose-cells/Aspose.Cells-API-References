---
title: CellArea.CreateCellArea
second_title: Aspose.Cells for .NET API Reference
description: CellArea method. Creates a cell area
type: docs
url: /net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Creates a cell area.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column. |
| endRow | Int32 | The end row. |
| endColumn | Int32 | The end column. |

### Return Value

Return a [`CellArea`](../).

### Examples

```csharp
// Called: fcc.Add(CellArea.CreateCellArea(0, 0, 1, 1),
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.Add(CellArea.CreateCellArea(0, 0, 1, 1),
                FormatConditionType.CellValue, OperatorType.Between, "abc def", "=\"a\"&\"b\"");
            FormatCondition fc = fcc[0];
            Assert.AreEqual("=\"abc def\"", fc.Formula1, "Text value of FormatCondition.Formula");
            Assert.AreEqual("=\"a\"&\"b\"", fc.Formula2, "Read FormatCondition.Formula");
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
            fc = wb.Worksheets[0].ConditionalFormattings[0][0];
            Assert.AreEqual("=\"abc def\"", fc.Formula1, "Text value of FormatCondition.Formula");
            Assert.AreEqual("=\"a\"&\"b\"", fc.Formula2, "Read FormatCondition.Formula");
            wb = Util.ReSave(wb, SaveFormat.SpreadsheetML);
            fc = wb.Worksheets[0].ConditionalFormattings[0][0];
            Assert.AreEqual("=\"abc def\"", fc.Formula1, "Text value of FormatCondition.Formula");
            Assert.AreEqual("=\"a\"&\"b\"", fc.Formula2, "Read FormatCondition.Formula");
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Creates a cell area.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |

### Return Value

Return a [`CellArea`](../).

### Examples

```csharp
// Called: CellArea ca = CellArea.CreateCellArea(startCell, endCell);
[Test]
        public void Method_String_()
        {
            String startCell = "$A$1"; String endCell = "$C$1";
            CellArea ca = CellArea.CreateCellArea(startCell, endCell);
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


