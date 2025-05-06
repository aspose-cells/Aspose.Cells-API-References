---
title: ErrorCheckOptionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOptionCollection property. Gets ErrorCheckOption object by the given index
type: docs
url: /net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Gets [`ErrorCheckOption`](../../errorcheckoption/) object by the given index.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Return Value

Return [`ErrorCheckOption`](../../errorcheckoption/) object

### Examples

```csharp
// Called: ErrorCheckOption optsummary  = optssummary[indexsummary];
[Test]
        public void Property_Int32_()
        {
            Workbook workBook = new Workbook();
            workBook.Worksheets[0].Cells[&quot;A1&quot;].PutValue(&quot;1111&quot;);
            workBook.Worksheets[0].Cells[&quot;A2&quot;].PutValue(&quot;double click A1,green color should not appear in the left corner.&quot;);
            ErrorCheckOptionCollection optssummary  = workBook.Worksheets[0].ErrorCheckOptions;
            int indexsummary  = optssummary.Add();
            ErrorCheckOption optsummary  = optssummary[indexsummary];
            optsummary.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            optsummary.SetErrorCheck(ErrorCheckType.EvaluationError, false);
            optsummary.SetErrorCheck(ErrorCheckType.CalculatedColumn, false);
            optsummary.SetErrorCheck(ErrorCheckType.EmptyCellRef, false);
            optsummary.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            optsummary.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            optsummary.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            optsummary.SetErrorCheck(ErrorCheckType.UnlockedFormula, false);
            optsummary.SetErrorCheck(ErrorCheckType.TableDataValidation, false);

            optsummary.AddRange(CellArea.CreateCellArea(0, 0, workBook.Worksheets[0].Cells.MaxRow, workBook.Worksheets[0].Cells.MaxDataColumn));
            workBook.Save(Constants.destPath + &quot;Cellnet43164.xlsx&quot;);
        }
```

### See Also

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


