---
title: Cells.MaxDataColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum column index of cell which contains data
type: docs
url: /net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Maximum column index of cell which contains data.

```csharp
public int MaxDataColumn { get; }
```

### Remarks

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### Examples

```csharp
// Called: Aspose.Cells.Range masterRange = ws.Cells.CreateRange(_startRow, 0, _numberOfRows, ws.Cells.MaxDataColumn);
[Test]
        public void Property_MaxDataColumn()
        {
            int _numberOfRows = 4;
            int _startRow = 9;
            string path = Constants.sourcePath + &quot;CellsNet31102.xls&quot;;
            Workbook wb = new Workbook(path);
            Worksheet ws = wb.Worksheets[0];

            //Get template range
            Aspose.Cells.Range masterRange = ws.Cells.CreateRange(_startRow, 0, _numberOfRows, ws.Cells.MaxDataColumn);
            Aspose.Cells.Range rng = null;
            PasteOptions po = new PasteOptions();
            po.PasteType = PasteType.All;
            //Add 500 dummy rows
            for (int j = 0; j &lt; 500; j+= _numberOfRows)
            {
                rng = ws.Cells.CreateRange(j + _startRow, 0, _numberOfRows, ws.Cells.MaxDataColumn);
                //Copy Range
                rng.Copy(masterRange, po);
                //Add row information ....
            }
            ws.CalculateFormula(new CalculationOptions() { IgnoreError = true }, true);
            Util.ReSave(wb, SaveFormat.Excel97To2003);
            //wb.Save(Constants.destPath + &quot;CellsNet31102.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


