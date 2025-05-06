---
title: Cells.ClearFormats
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears formatting of a range
type: docs
url: /net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Clears formatting of a range.

```csharp
public void ClearFormats(CellArea range)
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

## ClearFormats(int, int, int, int) {#clearformats_1}

Clears formatting of a range.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |

### Examples

```csharp
// Called: cells.ClearFormats(0, 0, 2, 2);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testClearFormats_001&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            Style style = GetStyle(workbook);

            for (int row = 0; row &lt; 3; row++)
            {
                for (int col = 0; col &lt; 3; col++)
                {
                    cells[row, col].SetStyle(style);
                    cells[row, col].PutValue(1);
                }
            }
            cells.ClearFormats(0, 0, 2, 2);

            checkClearFormats_001(workbook);
            workbook.Save(Constants.destPath + &quot;testClearFormats.xls&quot;);            
            workbook = new Workbook(Constants.destPath + &quot;testClearFormats.xls&quot;);
            checkClearFormats_001(workbook);
            workbook.Save(Constants.destPath + &quot;testClearFormats.xlsx&quot;);            
            workbook = new Workbook(Constants.destPath + &quot;testClearFormats.xlsx&quot;);
            checkClearFormats_001(workbook);
            workbook.Save(Constants.destPath + &quot;testClearFormats.xml&quot;, SaveFormat.SpreadsheetML);            
            workbook = new Workbook(Constants.destPath + &quot;testClearFormats.xml&quot;);
            checkClearFormats_001(workbook);
            workbook.Save(Constants.destPath + &quot;testClearFormats.xls&quot;);            
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


