---
title: ReferredArea.SheetName
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates which sheet this reference is in
type: docs
url: /net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Indicates which sheet this reference is in.

```csharp
public string SheetName { get; }
```

### Remarks

If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Examples

```csharp
// Called: Assert.Fail(&amp;quot;SheetName should be Sheet1 but was &amp;quot; + ra.SheetName);
[Test]
        public void Property_SheetName()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Formula/ExternalFormula.xls&quot;);
            ReferredArea ra = wb.Worksheets.Names[&quot;RefExternalName&quot;].GetReferredAreas(false)[0];
            if (!ra.ExternalFileName.EndsWith(&quot;ExternalLinkSource.xlsx&quot;))
            {
                Assert.Fail(&quot;ExternFileName should be ExternalLinkSource.xlsx but was &quot; + ra.ExternalFileName);
            }
            if (!ra.SheetName.Equals(&quot;Sheet1&quot;))
            {
                Assert.Fail(&quot;SheetName should be Sheet1 but was &quot; + ra.SheetName);
            }
            Assert.AreEqual(0, ra.StartRow, &quot;StartRow&quot;);
            Assert.AreEqual(0, ra.StartColumn, &quot;StartColumn&quot;);
            Assert.AreEqual(2, ra.EndRow, &quot;EndRow&quot;);
            Assert.AreEqual(2, ra.EndColumn, &quot;EndColumn&quot;);
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


