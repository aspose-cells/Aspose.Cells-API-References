---
title: CalculationOptions.IgnoreError
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function external links etc. The default value is true
type: docs
url: /net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

```csharp
public bool IgnoreError { get; set; }
```

### Examples

```csharp
// Called: ws.CalculateFormula(new CalculationOptions() { IgnoreError = true }, true);
[Test]
        public void Property_IgnoreError()
        {
            int _numberOfRows = 4;
            int _startRow = 9;
            string path = Constants.sourcePath + "CellsNet31102.xls";
            Workbook wb = new Workbook(path);
            Worksheet ws = wb.Worksheets[0];

            //Get template range
            Aspose.Cells.Range masterRange = ws.Cells.CreateRange(_startRow, 0, _numberOfRows, ws.Cells.MaxDataColumn);
            Aspose.Cells.Range rng = null;
            PasteOptions po = new PasteOptions();
            po.PasteType = PasteType.All;
            //Add 500 dummy rows
            for (int j = 0; j < 500; j+= _numberOfRows)
            {
                rng = ws.Cells.CreateRange(j + _startRow, 0, _numberOfRows, ws.Cells.MaxDataColumn);
                //Copy Range
                rng.Copy(masterRange, po);
                //Add row information ....
            }
            ws.CalculateFormula(new CalculationOptions() { IgnoreError = true }, true);
            Util.ReSave(wb, SaveFormat.Excel97To2003);
            //wb.Save(Constants.destPath + "CellsNet31102.xls");
        }
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


