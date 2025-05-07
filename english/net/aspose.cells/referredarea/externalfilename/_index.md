---
title: ReferredArea.ExternalFileName
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Get the external file name if this is an external reference
type: docs
url: /net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Get the external file name if this is an external reference.

```csharp
public string ExternalFileName { get; }
```

### Examples

```csharp
// Called: if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
[Test]
        public void Property_ExternalFileName()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Formula/ExternalFormula.xls");
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Assert.Fail("ExternFileName should be ExternalLinkSource.xlsx but was " + ra.ExternalFileName);
            }
            if (!ra.SheetName.Equals("Sheet1"))
            {
                Assert.Fail("SheetName should be Sheet1 but was " + ra.SheetName);
            }
            Assert.AreEqual(0, ra.StartRow, "StartRow");
            Assert.AreEqual(0, ra.StartColumn, "StartColumn");
            Assert.AreEqual(2, ra.EndRow, "EndRow");
            Assert.AreEqual(2, ra.EndColumn, "EndColumn");
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


