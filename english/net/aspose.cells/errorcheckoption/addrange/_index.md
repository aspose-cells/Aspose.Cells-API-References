---
title: ErrorCheckOption.AddRange
second_title: Aspose.Cells for .NET API Reference
description: ErrorCheckOption method. Adds one influenced range by this setting
type: docs
url: /net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Adds one influenced range by this setting.

```csharp
public int AddRange(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the range to be added. |

### Return Value

the index of the added range in the range list of this setting.

### Examples

```csharp
// Called: opts.AddRange(CreateCellArea("A1", "D2"));
public void ErrorCheckOption_Method_AddRange()
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

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


