---
title: Range.RefersTo
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the ranges refers to
type: docs
url: /net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Gets the range's refers to.

```csharp
public string RefersTo { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("=Sheet1!$G$4:$H$6", ranges[0].RefersTo);
public void Range_Property_RefersTo()
{
    Workbook book = new Workbook(Constants.sourcePath + "example.xlsx");
    book.Save(Constants.destPath + @"example.ods");
    book = new Workbook(Constants.destPath + @"example.ods");
    Name name = book.Worksheets.Names["abc"];
    Aspose.Cells.Range[] ranges = name.GetRanges();
    Assert.AreEqual("=Sheet1!$G$4:$H$6", ranges[0].RefersTo);
    Assert.AreEqual("=Sheet1!$J$8:$K$10", ranges[1].RefersTo);
    Assert.AreEqual("=SUM((A1,A5,A9))", book.Worksheets[0].Cells["F8"].Formula);
           
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


