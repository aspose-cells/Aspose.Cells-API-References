---
title: Worksheet.ErrorCheckOptions
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets error check setting applied on certain ranges
type: docs
url: /net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Gets error check setting applied on certain ranges.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Examples

```csharp
// Called: opt = workbook.Worksheets[0].ErrorCheckOptions[0];
[Test]
        public void Property_ErrorCheckOptions()
        {
            Workbook workbook = new Workbook();
            Worksheet s = workbook.Worksheets[0];
            Aspose.Cells.ErrorCheckOptionCollection opts = s.ErrorCheckOptions;

            int i = opts.Add();

            Aspose.Cells.ErrorCheckOption opt = opts[i];

            opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.NumberStoredAsText, false);
            opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.EvaluationError, false);
            //opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.EmptyCellRef, false);
            opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.UnlockedFormula, false);
            opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.TwoDigitTextYear, false);

            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 0;
            ca.EndColumn = 0;

            opt.AddRange(ca);
            workbook.Save(Constants.destPath + &quot;CellsNet40081.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet40081.xls&quot;);
            opt = workbook.Worksheets[0].ErrorCheckOptions[0];
            Assert.AreEqual(opt.IsErrorCheck(ErrorCheckType.NumberStoredAsText),false);
            workbook.Save(Constants.destPath + &quot;CellsNet40081.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet40081.xlsx&quot;);
            opt = workbook.Worksheets[0].ErrorCheckOptions[0];
            Assert.AreEqual(opt.IsErrorCheck(ErrorCheckType.NumberStoredAsText), false);
        }
```

### See Also

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


