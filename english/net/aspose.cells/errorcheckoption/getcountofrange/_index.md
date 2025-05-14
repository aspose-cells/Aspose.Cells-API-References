---
title: ErrorCheckOption.GetCountOfRange
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Gets the count of ranges that influenced by this setting
type: docs
url: /net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Gets the count of ranges that influenced by this setting.

```csharp
public int GetCountOfRange()
```

### Return Value

the count of ranges that influenced by this setting.

### Examples

```csharp
// Called: Assert.AreEqual(opts.GetCountOfRange(), 2);
public void ErrorCheckOption_Method_GetCountOfRange()
{
    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    ErrorCheckOptionCollection optss = sheet.ErrorCheckOptions;
    int index = optss.Add();
    ErrorCheckOption opts = optss[index];
    opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
    opts.AddRange(CreateCellArea("A1", "D2"));
    opts.AddRange(CreateCellArea("A3", "D3"));
    index = optss.Add();
    opts = optss[index];
    opts.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
    opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
    opts.AddRange(CreateCellArea("A3", "D5"));
    workbook.Save(Constants.destPath + "TestErrorCheck.xls");
    workbook = new Workbook(Constants.destPath + "TestErrorCheck.xls");
    sheet = workbook.Worksheets[0];
            
    Assert.AreEqual(sheet.ErrorCheckOptions.Count, 2);
    opts = sheet.ErrorCheckOptions[0];
    Assert.AreEqual(opts.GetCountOfRange(), 2);
    Assert.AreEqual(opts.IsErrorCheck(ErrorCheckType.NumberStoredAsText), false);

}
```

### See Also

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


