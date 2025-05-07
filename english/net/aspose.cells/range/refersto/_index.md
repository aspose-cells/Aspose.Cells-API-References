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
// Called: Assert.AreEqual("=Sheet1!$C$3:$D$5", rs[0].RefersTo, "First range");
[Test]
        public void Property_RefersTo()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Formula/AreasList.ods");
            Name n = wb.Worksheets.Names["test"];
            Assert.AreEqual("=Sheet1!$C$3:$D$5,Sheet1!$F$7:$H$9", n.RefersTo);
            Aspose.Cells.Range[] rs = n.GetRanges();
            Assert.AreEqual(2, rs.Length);
            Assert.AreEqual("=Sheet1!$C$3:$D$5", rs[0].RefersTo, "First range");
            Assert.AreEqual("=Sheet1!$F$7:$H$9", rs[1].RefersTo, "Second range");
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


