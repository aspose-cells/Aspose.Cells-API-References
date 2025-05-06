---
title: ListObject.PutCellFormula
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Put the formula to the cell in the table
type: docs
url: /net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Put the formula to the cell in the table.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| formula | String | The formula of the cell. |

### Examples

```csharp
// Called: table.PutCellFormula(4, 2, &amp;quot;=C3&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET53284.xlsx&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            ListObject table = wb.Worksheets[0].ListObjects[0];
            table.PutCellValue(4, 0, &quot;88&quot;);
            table.PutCellValue(4, 1, 88);
            table.PutCellFormula(4, 2, &quot;=C3&quot;);
            Assert.AreEqual(&quot;88&quot;, table.ListColumns[0].TotalsRowLabel);

            wb.Save(Constants.destPath + &quot;CELLSNET53284.xlsx&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Put the formula to the cell in the table.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| formula | String | The formula of the cell. |
| isTotalsRowFormula | Boolean |  |

### Examples

```csharp
// Called: l1.PutCellFormula(3, 0, &amp;quot;=23+34&amp;quot;, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet53358.xlsx&quot;);
            ListObject l0 = workbook.Worksheets[0].ListObjects[0];
            l0.PutCellFormula(3, 0, &quot;=23+34&quot;, false);
            Assert.AreEqual(4, l0.EndRow);
            ListObject l1 = workbook.Worksheets[1].ListObjects[0];
            l1.PutCellFormula(3, 0, &quot;=23+34&quot;, true);
            Assert.AreEqual(3, l1.EndRow);
            Assert.AreEqual(&quot;=23+34&quot;, workbook.Worksheets[1].Cells[&quot;A4&quot;].Formula);
            ListObject l2 = workbook.Worksheets[2].ListObjects[0];
            l2.PutCellValue(3, 2, &quot;sdfsfdsfd&quot;, true);

            Assert.AreEqual(3, l2.EndRow);
            Assert.AreEqual(&quot;sdfsfdsfd&quot;, workbook.Worksheets[2].Cells[&quot;C4&quot;].StringValue);

            workbook.Save(Constants.destPath + &quot;CellsNet53358.xlsx&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


