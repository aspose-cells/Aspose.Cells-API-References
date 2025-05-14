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
// Called: fcc.RemoveArea(1);
public void FormatConditionCollection_Method_RemoveArea()
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
// Called: fcc.RemoveArea(row, col, 1, 1);
public void FormatConditionCollection_Method_RemoveArea()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
    string[] formulas = new string[]
    {
        "=$C$8=$C$7", "=$E$8=$E$7", "=$F$8=$F$7", "=$G$8=$G$7", "=$C$7=$C$6", "=$E$7=$E$6",
        "=$F$7=$F$6", "=$G$7=$G$6", "=$B$7=$B$5", "=$D$7=$D$6", "=$D$8=$D$7"
    };
    string[] initialCells = new string[]
    {
        "C8", "E8", "F8", "G8", "C7", "E7", "F7", "G7", "B7", "D7", "D8"
    };
    Random rand = new Random();
    TimePerformance monitor = new TimePerformance(30);
    monitor.StartPerfTest();
    for (int i = 0; i < formulas.Length; i++)
    {
        int idx = cfc.Add();
        FormatConditionCollection fcc = cfc[idx];
        int row, col;
        CellsHelper.CellNameToIndex(initialCells[i], out row, out col);
        CellArea ca = CellArea.CreateCellArea(row, col, row, col);
        fcc.AddArea(ca);

        idx = fcc.AddCondition(FormatConditionType.Expression);
        FormatCondition fc = fcc[idx];
        fc.Formula1 = formulas[i];
        fc.Style.Font.Color = Color.FromArgb(0, 97, 0);
        Console.WriteLine("Processing condition: " + fcc[0].Formula1);
        // create single cell areas for about 1000 cells
        for (int j = 0; j < 1000; j++)
        {
            row = rand.Next(20000);
            col = rand.Next(26);
            fcc.RemoveArea(row, col, 1, 1);
            // Add the cell to the collection in order to apply conditional formatting
            CellArea area = CellArea.CreateCellArea(row, col, row, col);
            fcc.AddArea(area);
        }
    }
    monitor.FinishPerfTest("Repeatedly remove and add areas for 1000 times");
}
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


