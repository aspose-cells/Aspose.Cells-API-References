---
title: Name.GetReferredAreas
second_title: Aspose.Cells for .NET API Reference
description: Name method. Gets all references referred by this name
type: docs
url: /net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Gets all references referred by this name.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |

### Return Value

All ranges.

### Examples

```csharp
// Called: ReferredArea ra = wb.Worksheets.Names[&amp;quot;RefExternalName&amp;quot;].GetReferredAreas(false)[0];
[Test]
        public void Method_Boolean_()
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

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


