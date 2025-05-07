---
title: FormatConditionCollection.RemoveArea
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Removes conditional formatted cell range by index
type: docs
url: /net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Removes conditional formatted cell range by index.

```csharp
public void RemoveArea(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the conditional formatted cell range to be removed. |

### Examples

```csharp
// Called: fcc.RemoveArea(0);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 18, 1048575, 16382));
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1048570, 17));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;
            Cells cells = sheet.Cells;
            Random r = new Random();
            int[] flags = new int[1000];
            for (int i = 0; i < 128; i++)
            {
                for (int j = 0; j < 16; j++)
                {
                    int v = r.Next(flags.Length);
                    int f = flags[v];
                    if (f == 0)
                    {
                        cells[i, j].PutValue("U" + v);
                        flags[v] = ((i << 4) | j) + 1;
                    }
                    else
                    {
                        cells[i, j].PutValue("D" + v);
                        if (f > 0)
                        {
                            f--;
                            cells[f >> 4, f & 0x0F].PutValue("D" + v);
                            flags[v] = -1;
                        }
                    }
                }
            }
            flags = null;
            VerifyJ43108(wb);
            fcc.RemoveArea(1);
            fcc.RemoveArea(0);
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1048500, 16382));
            VerifyJ43108(wb);
            fcc.AddArea(CellArea.CreateCellArea(1048502, 0, 1048575, 16380));
            VerifyJ43108(wb);
            fcc.RemoveArea(1);
            fcc.RemoveArea(0);
            fcc.AddArea(CellArea.CreateCellArea(10, 5, 1048575, 16382));
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 9, 16382));
            fcc.AddArea(CellArea.CreateCellArea(10, 0, 1048575, 4));
            VerifyJ43108(wb);
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Remove conditional formatting int the range.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The startRow of the range. |
| startColumn | Int32 | The startColumn of the range. |
| totalRows | Int32 | The number of rows of the range. |
| totalColumns | Int32 | The number of columns of the range. |

### Return Value

Returns TRUE, this FormatCondtionCollection should be removed.

### Examples

```csharp
// Called: formatCollection.RemoveArea(row, col, 1, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook wk = new Workbook(Constants.sourcePath + "ConditionalFormattings/CELLSJAVA42720.xlsx");
            DateTime dt = DateTime.Now;
            ConditionalFormattingCollection asposeFormattingCollection = wk.Worksheets[0].ConditionalFormattings;

            //long start = System.currentTimeMillis();
            for (int row = 16; row < 3000; row++)
            {
                for (int col = 2; col < 12; col++)
                {
                    FormatConditionCollection formatCollection = asposeFormattingCollection[0];
                    formatCollection.RemoveArea(row, col, 1, 1);
                    CellArea area = CellArea.CreateCellArea(row, col, row, col);
                    formatCollection.AddArea(area);
                }
            }
            Assert.AreEqual(2,asposeFormattingCollection[0].RangeCount);
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


