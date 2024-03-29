---
title: Class ErrorCheckOption
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ErrorCheckOption class. Error check setting applied on certain ranges
type: docs
url: /net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Error check setting applied on certain ranges.

```csharp
public class ErrorCheckOption
```

## Methods

| Name | Description |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Adds one influenced range by this setting. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Gets the count of ranges that influenced by this setting. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Gets the influenced range of this setting by given index. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Checks whether given error type will be checked. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Removes one range by given index. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Sets whether given error type will be checked. |

### Examples

```csharp

[C#]

  Workbook workbook = new Workbook();
  ErrorCheckOptionCollection opts = workbook.Worksheets[0].ErrorCheckOptions;
  int optionIdx = opts.Add();
  ErrorCheckOption opt = opts[optionIdx];
  opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.InconsistFormula, false);
  opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.InconsistRange, false);
  opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.TextDate, false);
  opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.TextNumber, false);
  opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.Validation, false);
  opt.AddRange(CellArea.CreateCellArea("A1", "B10"));
  workbook.Save(@"Book1.xlsx");
  
[Visual Basic]

   Dim workbook As Workbook = New Workbook()
   Dim opts As ErrorCheckOptionCollection = workbook.Worksheets(0).ErrorCheckOptions
   Dim optionIdx As Integer = opts.Add()
   Dim opt As ErrorCheckOption = opts(optionIdx)
   opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.InconsistFormula, False)
   opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.InconsistRange, False)
   opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.TextDate, False)
   opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.TextNumber, False)
   opt.SetErrorCheck(Aspose.Cells.ErrorCheckType.Validation, False)
   opt.AddRange(CellArea.CreateCellArea("A1", "B10"))
   workbook.Save("Book1.xlsx")
   
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


