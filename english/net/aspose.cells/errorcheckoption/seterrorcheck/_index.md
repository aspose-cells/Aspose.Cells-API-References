---
title: ErrorCheckOption.SetErrorCheck
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Sets whether given error type will be checked
type: docs
url: /net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Sets whether given error type will be checked.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | error type can be checked. |
| isCheck | Boolean | true if given error type needs to be checked(green triangle will be shown for cell if the check failed). |

### Examples

```csharp
// Called: optsummary.SetErrorCheck(ErrorCheckType.TableDataValidation, false);
public void ErrorCheckOption_Method_SetErrorCheck()
{
    Workbook workBook = new Workbook();
    workBook.Worksheets[0].Cells["A1"].PutValue("1111");
    workBook.Worksheets[0].Cells["A2"].PutValue("double click A1,green color should not appear in the left corner.");
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
    workBook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


