---
title: ErrorCheckOption.IsErrorCheck
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Checks whether given error type will be checked
type: docs
url: /net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

Checks whether given error type will be checked.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | error type can be checked |

### Return Value

return true if given error type will be checked(green triangle will be shown for cell if the check failed).

### Examples

```csharp
// Called: Assert.AreEqual(opt.IsErrorCheck(ErrorCheckType.NumberStoredAsText),false);
public void ErrorCheckOption_Method_IsErrorCheck()
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
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    opt = workbook.Worksheets[0].ErrorCheckOptions[0];
    Assert.AreEqual(opt.IsErrorCheck(ErrorCheckType.NumberStoredAsText),false);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    opt = workbook.Worksheets[0].ErrorCheckOptions[0];
    Assert.AreEqual(opt.IsErrorCheck(ErrorCheckType.NumberStoredAsText), false);
}
```

### See Also

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


