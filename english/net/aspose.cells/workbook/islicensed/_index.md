---
title: Workbook.IsLicensed
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Indicates whether license is set
type: docs
url: /net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Indicates whether license is set.

```csharp
public bool IsLicensed { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(wb.IsLicensed, "Should be licensed");
[Test]
        public void Property_IsLicensed()
        {
            License license = new License();
            license.SetLicense(Constants.licPath);
            Workbook wb = new Workbook();
            Assert.IsTrue(wb.IsLicensed, "Should be licensed");
            wb.Worksheets[0].Cells[0, 0].PutValue("Licensed version test");
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
            Assert.AreEqual(1, wb.Worksheets.Count, "Licensed version");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


